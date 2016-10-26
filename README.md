# riddle

![](https://img.shields.io/npm/v/riddles.svg?style=flat-square)
![](https://img.shields.io/npm/l/riddles.svg?style=flat-square)

A framework for building an online puzzle-solving system, like Python Challenge.

## Features

Users & groups & problems management, quizzes orders (拓扑序), real-time submissions, ranking board, etc. 

Designed to be simple and responsive.

## Install
- install NodeJS and MongoDB
- `npm install riddles`

You can modify your settings in `config.json`, change the default HTTP port in `bin/www` line 15 (or use an environment variable).

## Usage
- Start MongoDB
- run `npm start`

Currently you must manually modify the `group` field from `user` to `admin` of all administrators in DB to make it work.  

For example, you can just run this in your mongo shell:  
`db.users.update({ _id: ObjectId("57fcd7ce763xxxxxxc3476") }, { $set: { group: "admin" } } )`

## Screenshots

![screenshot/1.png](screenshot/1.png)

![screenshot/2.png](screenshot/2.png)

Reordering puzzles
![screenshot/3.png](screenshot/3.png)

## About
Author: Shu Ding  
License: MIT  
Production info: This framework was used in 复旦推协's annual online-offline puzzle-solving event. 
