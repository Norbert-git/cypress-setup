Cypress Setup

Create a folder

- npm init -y ( will create a package.json file)
- npm install cypress@9.5.4 --save -dev
- npx cypress open ( will create cypress folder and some example file)

Cypress.json

    {
    	"baseUrl": "https://google.com",
    	"chromeWebSecurity": false,
    	"ignoreTestFiles": "**/examples/*",
    	"viewportHeight": 1080,
    	"viewportWidth": 1920,
    	"testFiles": "**/*.spec.js"
    }
    
    
    ( for "baseUrl": "https://localhost:4200", )
    ( change the testFiles according to what file type you using )

Package.json

    "scripts": {
    		"test": "cypress open"
    }
    
    
    ( This is optional, it will allow you to run cypress with the command:
    npm run test )

Add .gitignore file

Add README.md file
