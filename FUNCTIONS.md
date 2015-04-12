Functions
=========

##Send SMS
  * Name: "send_sms"<br>
  * Action: Send to all contacts in android host or send to assign numbers<br>
  
  ####Controller:
      JSON:
      {
           "only": [], // numbers to send. if null, send to all contacts
           "content": "string" // SMS content
      }
  ####Host:
      Null

##Load Contacts
  * Name: "load_contact"<br>
  * Action: Load all contacts from android host
  
  ####Controller:
  
      Null
    
  ####Host:
      JSON: 
      {
          "upload_contacts": [
              "number1", "number2", .....
          ]
      }

##Load SMS
  * Name: "upload_sms"<br>
  * Action: Load all SMS from android host
  
  ####Controller:
  
      Null
      
  ####Host:
      JSON: 
      {
          "upload_sms": [
              object(sms infomation),  object(sms infomation2),.....
          ]
      }


##Shell
  * Name: "shell"<br>
  * Action: Open a shell of android host
  
  ####Controller:
  
      Text stream, end with '\n'
      
  ####Host:
  
      Text stream, all of shell stdout & stderr.
