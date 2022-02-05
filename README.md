# GraphqlNotes

query {

  allLifts{

    name

   status

  }

  }

 

mutation{

  createAccount(input: {

    name: "Me"

    username: "Yoitsme"

    password:"pwrd"

  }) {

    username

    name

  }

}

 

 

Or, could add input:

mutation ($input:CreateAccountInput!){

  createAccount(input:$input){

    username

    name

  }

}

 

{

  "input": {

            "name": "You",

    "username": "Heyyy",

    "password":"pass"

}

}

 
