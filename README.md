# validate_cc

Semester_validation	
OR(Semester__c >8,Semester__c <=0)

CGPA_validation	
Formula	CGPA__c >10

Student_Name_Validation	
Formula	NOT(REGEX(Name,"[a-z A-Z]+[a-z A-Z]+"))

USN_Validation	
Formula	NOT(REGEX(USN__c,"[1-5]{1}+[A-Z]{2}+[0-9]{2}+[A-Z]{2}+[0-9]{3}"))

staff_id_validation	
Error Condition Formula	NOT ( BEGINS( Id__c ,'STAFF')

Date_Time_should_be_in_Range	Active	Checked
Error Condition Formula	Departure_Timings__c <NOW ()

Source_and_destination_Checking	Active	Checked
Error Condition Formula	Source__c = Destination__c
