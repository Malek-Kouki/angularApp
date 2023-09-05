## Lessons

1. Install development tools
2. Create Angular App
   1. Create project's folder (mkdir foodmine)
   2. Install @angular/cli
   3. Create App as frontend (ng new frontend --skip-tests)
   4. Remove git folder (rm -rf .git)
   5. Initialize Repository :
      > Icon source Control
      > Initialize Repository
      > Create Angular App.
      > ✔
      > Publish Bransh
      > Continue
      > Open with VsCode
      > Name : foodmine-app
      > Push to Github public
      > Open on Github

3. Add Header
   1. Generate Component
   2. Add Html
   3. Add CSS

4. List Foods
   1. Create Food model (food.ts)
   2. Create data.ts
      1. Add sample foods (data base to test)
   3. Add images to assets
   4. Create Food service
      > getAll
   5. Create Home component
      1. Add ts
         > Appel 'Food service'
      2. Add html
      3. Add css
   6. Create starRating component
      1. Add ts
      2. Add html
      3. Add css

5. Search
   1. Add method to Food service
      > getAllFoodsBySearchTerm
   2. Add search route (app-routing.module.ts)
   3. Show search result in Home component
      > change "noPropertyAccessFromIndexSignature": false (tconfig.json)
      > activatedRoute (home.component.ts)
   4. Generate search component
      1. Add to home component
      2. Add ts
      3. Add html
      4. Add css

6. Food Page
   1. Add method to food service
      > getFoodById
   2. Generate Food Page component
      1. Add Route
      2. Add ts
      3. Add html
      4. Add css

7. Tags Bar
   1. Create Tag model
   2. Add sample tags to data.ts
   3. Food service
      1. Add get all tags method
      2. Add get all foods by tag method
   4. Add tags route
   5. Show tag result in Home component
   6. Generate Tags component
      1. Add to home component
      2. Add ts
      3. Add html
      4. Add css

8. Cart Page
   1. Create CartItem Model
   2. Create Cart Model
   3. Generate Cart service
   4. Add to Cart Button in Food Page 
      > addToCart (food-page.ts + food-page.html) 
   5. Generate Cart page component
      1. Add Route
      2. Add ts
      3. Add html
      4. Add css

9. Not Found!
   1. Generate Component
      1. Add ts
      2. Add html
      3. Add css
   2. Add To Pages
      1. Home Page
      2. Food Page
      3. Cart Page

10. Connect To Backend
   1.  Create backend folder
   2.  npm init (npm init -y)
   3.  npm install typescript
   4.  Create tsconfig.json
   5.  Create .gitignore
   6.  Copy data.ts to backend/src
   7.  npm install express cors
   8.  Create server.ts
      1. install @types
         > npm install --save-dev @types/express
         > npm install --save-dev @types/cors
      2. npm install nodemon ts-node --save-dev
      3. npm install nodemon --save-dev (npm start : lancer le serveur)
      2. Add Apis
   9.  Add urls.ts to frontend
   10. Add HttpClient module
   11. Update food service
   12. Update home.ts + food-page.ts + tags.ts

11. Login Page
   1. Generate Component
      1. Add to routes
      2. Add ts 
      3. Add html
         1. Import Reactive Forms Module
      4.  Add Css
   2. Add Login Api (server.ts)
      1. Use json
      2. Add jsonwebtoken (npm install jsonwebtoken) 
      3. Test Using Postman
         >> Open Postman
         >> POST >> localhost:5000/api/users/login
         >> Body >> raw >> JSON
               {
                  "email": "jane@gmail.com",
                  "password": "12345"
               }
         >> Send
   3. Generate User Service
      1. Generate User model
      2. Add User Subject
      3. Add Login Method   
         1. Add User Urls
         2. Generate IUserLogin interface
         3. Add ngx-toastr
            1. Import Module
            2. Import BrowserAnimationsModule
            3. Add styles in angular.json
            4. Add to Header
         4. Add Local Storage methods 
            > setUserToLocalStorage (user.service.ts)
         5. header.ts + header.html
         6. Add Logout Method
            > logout (user.service.ts)
            > Add to Header (html + ts)

12. Make Components For Login Page
   1. Input Container
   2. Input Validation
   3. Text Input
   4. Default Button