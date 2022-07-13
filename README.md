# TUTORIAL : IMAGE-UPLOAD-MULTER

The tutorial on how to implement image uploads using Express and Multer with postgres sql as the database

## How to Run

1. Setting up a database

```
# Create image_upload postgres database
$ createdb image_upload

# Create image_files table
$ psql -d image_upload -a -f ./postgres/image_upload.sql

# Check
$ psql image_upload
$ image_upload=# \d
```

2. Install dependencies and run express server

```
$ npm install
$ npm start
```

3. API use guide

GET by filename
http://localhost:5002/image/:filename

POST image
http://localhost:5002/image

use postman
with 'image' as a key and type files,
select value with any image files.

