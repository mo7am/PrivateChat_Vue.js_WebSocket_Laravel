## PrivateChat_Vue.js_WebSocket_Laravel.

## get it up and running.

After you clone this project, do the following:

```bash
# go into the project
cd PrivateChat_Vue.js_WebSocket_Laravel

# create a .env file
copy .env.example file and rename it into .env 

# install composer dependencies
composer update

# install npm dependencies
npm install

# generate a key for your application
php artisan key:generate

# create a local MySQL database (make sure you have MySQL up and running)

# add the database connection config to your .env file
DB_CONNECTION=mysql
DB_DATABASE=your Database Name
DB_USERNAME=your Username
DB_PASSWORD=your Password

# run the migration files to generate the schema
php artisan migrate

## Setup pusher
- visit [Pusher website](https://pusher.com) , sign up and create your first app (it's free). 
- Next. copy the new keys to your `.env` file.
- Make sure the necessary settings are enabled
![Pusher app settings](https://user-images.githubusercontent.com/17595033/64108972-fb7b8a00-cd86-11e9-97ab-d2a3f7699b71.png)

PUSHER_APP_ID=your_pusher_app_id
PUSHER_APP_KEY=your_pusher_app_key
PUSHER_APP_SECRET=your_pusher_app_secret
PUSHER_APP_CLUSTER=your_pusher_cluster

# change the BROADCAST_DRIVER in your .env to pusher
BROADCAST_DRIVER=pusher

# run npm and watch for changes
npm run watch

# run server 
php artisan serve


# run websockets 
php artisan websocket:serve


# regist with user in opened browser
# regist with another user in new incognito window 

# Let's Chatting

Good Luck :)


















