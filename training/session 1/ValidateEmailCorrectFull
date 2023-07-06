
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
  
  // Array to hold new leads without duplicates
  var uniqueNewLeads = [];
  
  // Start from the second row to ignore the header
  for(var j = 1; j < newLeadsData.length; j++) {
    var currentEmail = newLeadsData[j][0].toLowerCase(); // Convert email to lower case
    // If the current email doesn't exist in the master list, add the row to uniqueNewLeads array
    if(!(currentEmail in masterEmailDict)) {
      uniqueNewLeads.push(newLeadsData[j]);
    }
  }

  // Clear previous data in 'new leads without duplicates' tab only if it contains data
  if(newLeadsNoDupSheet.getLastRow() > 1) {
    newLeadsNoDupSheet.getRange(2, 1, newLeadsNoDupSheet.getLastRow()-1, newLeadsNoDupSheet.getLastColumn()).clearContent();
  }
  
  // Write uniqueNewLeads to 'new leads without duplicates' tab
  if(uniqueNewLeads.length > 0) {
    newLeadsNoDupSheet.getRange(2, 1, uniqueNewLeads.length, uniqueNewLeads[0].length).setValues(uniqueNewLeads);
  }
}
