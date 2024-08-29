Dotenv use for the like variable use from the outside of the current file 
like mere pass .env file hai us k ander mene mera PORT number d diya hai or m mere index_file se uss ko acess kar rha hu 
#index.js
require('dotenv').config();
console.log(process.env.SECURITY_KEY);

#.env
SECURITY_KEY = "990jiuutbbfty667";

why we use Process.env file
 Standard Node.js Convention:
 
 Global Accessibility:
process.env is accessible globally throughout your Node.js application,
meaning you can access environment variables in any file or module,
regardless of where the dotenv configuration is set up.

Security:
