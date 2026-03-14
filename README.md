# MistiGameProject
Advanced Pisti Game Project

Overview

This project is a console-based implementation of the Mişti card game, a variation of the traditional Pişti game. The program simulates a full card game with human and AI players, score calculation, and game rounds.

The game is played with a standard 52-card deck and supports 2–4 players, including bots with different skill levels.

Features
Deck Management

Creates a standard 52-card deck

Shuffles and cuts the deck before each round

Deals cards to players and places cards on the board

Game Mechanics

Players take turns placing cards on the board

If a played card matches the value of the top card, the player takes all cards from the board

Jack cards can take all cards regardless of the top card

Mişti Rule

If a player captures only one card from the board, it counts as a Mişti, and the points of those cards are multiplied by five.

Score System

Card points are read from a points configuration file.
If a card does not match any rule in the file, it receives a default value of 1 point.

Player Types

The game supports different player behaviors:

Human Player – chooses cards through console input

Novice Bot – plays random cards

Regular Bot – chooses cards based on board value and potential score

Expert Bot – uses a more advanced strategy and tracks played cards

Game Output

The program prints game logs to the console, including:

Hands dealt to players

Cards played each turn

Round results and scores

Two modes are supported:

Verbose mode – detailed move logs

Succinct mode – only round scores

High Score System

The program maintains a Top 10 high score list stored in a file, including:

Player names

Player expertise level

Scores

The list updates automatically when a new score enters the top 10.

Concepts Used

Object-Oriented Programming (OOP)

File input/output

Game logic design

Collections and card management

Console interaction

Basic AI strategies

Git version control

How to Run

The program runs from the command line with parameters such as:

points file name

number of players

number of rounds

player names and types

Example:

java -jar misti.jar points.txt 3 5 Player1:human Bot1:novice Bot2:expert
Goal

The goal of this project is to implement a fully functional card game while practicing Java programming, object-oriented design, file handling, and simple AI strategies.
