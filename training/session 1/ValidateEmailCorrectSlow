function copyUniqueLeads() {
  var ss = SpreadsheetApp.openById('1EBSwlbsk6yZd100NH0e4wpd4o07ZELXYLTMrYDv9reY');
  
  var masterSheet = ss.getSheetByName('validated master list');
  var newLeadsSheet = ss.getSheetByName('new leads');
  var newLeadsNoDupSheet = ss.getSheetByName('new leads without duplicates');
  
  // Get data from the sheets
  var masterData = masterSheet.getDataRange().getValues();
  var newLeadsData = newLeadsSheet.getDataRange().getValues();

  // Create a dictionary with email as the key from master list
  var masterEmailDict = {};
  for(var i = 1; i < masterData.length; i++) {
    var lowerCaseEmail = masterData[i][0].toLowerCase(); // Convert email to lower case
    masterEmailDict[lowerCaseEmail] = masterData[i];
  }
  
  // Start from the second row to ignore the header
  for(var j = 1; j < newLeadsData.length; j++) {
    var currentEmail = newLeadsData[j][0].toLowerCase(); // Convert email to lower case
    // If the current email doesn't exist in the master list, copy the row to the 'new leads without duplicates' tab
    if(!(currentEmail in masterEmailDict)) {
      newLeadsNoDupSheet.appendRow(newLeadsData[j]);
    }
  }
}
