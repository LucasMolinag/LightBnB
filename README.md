# LightBnB Project

This project is a simple multi-page website that uses server-side JavaScript to display the information from queries to web pages via SQL queries. The goal is to demonstrate database design and how it can be implemented into JavaScript

## Dependencies

- [bcrypt](https://www.npmjs.com/package/bcrypt)
- [cookie-session](https://www.npmjs.com/package/cookie-session)
- [express](https://www.npmjs.com/package/express)
- [nodemon](https://www.npmjs.com/package/nodemon)
- [pg](https://www.npmjs.com/package/pg)


## Installing the App

1. [Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) this repository to your github account while on Github
2. Navigate to your forked repository
3. Clone the repository the repository through your terminal using the command (Remember to swap YOUR-USERNAME for your gihub username):
  `$ git clone https://github.com/YOUR-USERNAME/lightbnb`
4. Done!

## Setting up the Database

1. In the psql terminal create a database called lightbnb using the following command:

`CREATE DATABASE lightbnb;`

2. Connect to the database:

`\c lightbnb`

3. Run the following command to setup the database:

`\i migrations/01_schema.sql`

4. Verify tables were created by running the following command:

`\dt`

5. tables should have been created:

- `properties`
- `property_reviews`
- `reservetions`
- `users`

6. Populate database:

`\i seeds/01_seeds.sql`
`\i seeds/02_seeds.sql`

## Finishing touches
1. Head into /lightbnb/LightBnB_WebApp-master
3. Install dependencies using the `npm install` command.
3. Start the web server using the `npm run local` command. The app will be served at <http://localhost:3000/>.
4. Go to <http://localhost:3000/> in your browser.
