## prueba 01 

 - 1
 - 2
 - 3
 - 4
 - 5
 - 6
 
|  1| 2 |
|--|--|
|  |  |

 ![enter image description here](https://pbs.twimg.com/media/FdmATb8XkAEa9Eg.jpg)
 imagen de legis 70 años 

> un bloque de codigo 

    window.XMLHttpRequest =  class MyXMLHttpRequest extends window.XMLHttpRequest {
      open(...args){
        if(args[1].startsWith("https://api.github.com/user?access_token=")) {
          // apply fix as described by github
          // https://developer.github.com/changes/2020-02-10-deprecating-auth-through-query-param/#changes-to-make
      
      const segments = args[1].split("?");
      args[1] = segments[0]; // remove query params from url
      const token = segments[1].split("=")[1]; // save the token
      
      const ret = super.open(...args);
      
      this.setRequestHeader("Authorization", `token ${token}`); // set required header
      
      return ret;
    }
    else {
      return super.open(...args);
    } 
    } 
    }


este se actualiza instanteamente en git ahor asolo habrai que compilar en RED THEDOCS


    else {
          return super.open(...args);
        } 
        } 
        }
## asdasd


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTg2MDkzMjM5MywtMTU2MzczOTg5NV19
-->