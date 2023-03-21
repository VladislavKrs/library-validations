# library-validations


function validateLogin(loginVal, pattern, minLength, maxLength) {
  
  if(loginVal.length <= minLength || loginVal.length >= maxLength) {
   
    return false;

  } else if(!loginVal.match(pattern) == true) {
    
    return false;

  } else {
    
    return true;
  }
}

loginVal - принимет значение инпута login;

pattern - принимает регулярные выражения;

minLength - минимальное количество значение при вводе;

maxLength - максимальное количество значение при вводе;


function validateEmail(emailVal, pattern) {
 
  if(emailVal.match(pattern)) {
   
    return true

  } else {

    return false

  }
}

emailValue - принимет значение инпута email;

pattern - принимает регулярные выражения;

function validatePassword(passwordVal, pattern) {
 
  if(pattern.test(passwordVal)) {
   
    return true;

  } else {

    return false;

  }
}

passwordValue - принимет значение инпута password;

pattern - принимает регулярные выражения;
