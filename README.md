# Hostel-Registration-

function validate()
{ 
   if( document.HostelRegistration.textnames.value == "" )
   {
     alert( "Please provide your Name!" );
     document.HostelRegistration.textnames.focus() ;
     return false;
   }
   if( document.HostelRegistration.fathername.value == "" )
   {
     alert( "Please provide your Father Name!" );
     document.HostelRegistration.fathername.focus() ;
     return false;
   }
   if( document.HostelRegistration.haddress.value == "" )
   {
     alert( "Please provide your Home Address!" );
     document.HostelRegistration.haddress.focus() ;
     return false;
   }
   if ( ( HostelRegistration.sex[0].checked == false ) && ( HostelRegistration.sex[1].checked == false ) )
   {
   alert ( "Please choose your Gender: Male or Female" );
   return false;
   }      
   if( document.HostelRegistration.State.value == "-1" )
   {
     alert( "Please provide your Select State!" );
     return false;
   }
   if( document.HostelRegistration.pincode.value == "" ||
           isNaN( document.HostelRegistration.pincode.value) ||
           document.HostelRegistration.pincode.value.length != 6 )
   {
     alert( "Please provide a pincode in the format ######." );
     document.HostelRegistration.pincode.focus() ;
     return false;
   }
 var email = document.HostelRegistration.emailid.value;
  atpos = email.indexOf("@");
  dotpos = email.lastIndexOf(".");
 if (email == "" || atpos < 1 || ( dotpos - atpos < 2 )) 
 {
     alert("Please enter correct email ID")
     document.HostelRegistration.emailid.focus() ;
     return false;
 }
  if( document.HostelRegistration.dob.value == "" )
   {
     alert( "Please provide your DOB!" );
     document.HostelRegistration.dob.focus() ;
     return false;
   }
  if( document.HostelRegistration.mobileno.value == "" ||
           isNaN( document.HostelRegistration.mobileno.value) ||
           document.HostelRegistration.mobileno.value.length != 10 )
   {
     alert( "Please provide a Mobile No in the format 123." );
     document.HostelRegistration.mobileno.focus() ;
     return false;
   }

 alert("Form Submitted");
   return( true );
	
}
