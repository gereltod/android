# Ажиллах орчин үүсгэх

#### 1. Node.js санг суулгана. Javascript дээр суурилсан програмчлалын хэлүүд нь энэхүү сан дээр сууриллаж ажилладаг.

## Node.js суулгах
    Татах хаяг[https://nodejs.org/en/download/](https://nodejs.org/en/download/)
    Өөрийн үйлдлийн системд таарсан хувилбараа татаж авч суулгана.
    Амжилттай суулгасан бол. Терминал, powershell, cmd аль байгаа дээрээ 
    node -v
    npm -v 
    Энэхүү коммандууд хэвийн ажиллаж суулгасан хувилбарыг харуулна.


## How to install

    git clone https://github.com/evheniy/react-awesome-app.git
    cd react-awesome-app
    npm i
    
## How to run databases with docker

#### Start:
    
    npm run db:start
    
#### Stop:

    npm run db:stop
    
## How to run server 

### Node.js

#### Start ([http://localhost:3000/](http://localhost:3000/)):

    npm run server:start
    
#### Stop:

    npm run server:stop
    
### Docker

#### Build:

    npm run docker:build
    
#### Run ([http://localhost/](http://localhost/)):

    npm run docker:run

#### Stop:

    npm run docker:stop
    
### Docker Compose

#### Run ([https://localhost/](https://localhost/)):

    npm run compose:up
    
#### Stop:

    npm run compose:down

#### Clear:

    npm run compose:clear
    
### URLs to test

| Action       | Method | Path           | Request             | Response           |
|--------------|--------|----------------|---------------------|--------------------|
| Registration | POST   | /users         | { email, password } | { user, error }    |
| Login        | POST   | /tokens        | { email, password } | { token, error }   |
| User list    | GET    | /users         | { token }           | { users[], error } |
| User profile | GET    | /users/:id     | { token }           | { user, error }    |
| User editing | PATCH  | /users/:id     | { token, password } | { user, error }    |
| Logout       | DELETE | /tokens/:token | { token }           | { empty, error }   |

### GraphQL

#### URL: [/graphql](https://localhost/graphql)

## How to test

    npm t
    
## Clear docker

    npm run clear
