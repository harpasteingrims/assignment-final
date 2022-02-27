# Assignment Final

#### The full circle

---

This is it. The Big one. Now it's time to put all our learnings into one final project. In this assignment you will be setting up a CD pipeline with all the steps done in previous assignments. You will be setting up a staging environment along with a production environment. Your application will be deployed to the staging environment and from there it can be promoted to production.

What you will be working with is a Tic Tac Toe game that needs maintenance. Some logic is needed to complete the game and it is untested, some libraries are outdated and need to be updated.

The Project is a NextJS application with a Postgres database to keep track of the games.

**Please remember** to commit and push often (meaningful commits), the Git history is part of the assignment.

**Group size**: 1 person

---

## The Assignment

#### **Fix it!**

- Currently the game can only tell when someone wins, but not when there is a draw. Write a test for such function and then implement it and add that to the game.
- Should the game be playable without the players names ?
- There is an outdated library there somewhere, can you spot it ?
- There are no unit tests. Add them.
- There are no ui integration tests. Add them.
- There are no e2e tests. Add them.

#### **Deploy it!**

- Create a Github action that does all the checks we've been doing in previous assignments and then deploys the application to a staging environment. Where then, if staging deployment is successful, it can be promoted to a production environment. Please note the checks should be done on any branch but the deployment should only happen on the `main` branch.
- When deploying it should be deploying a docker image that has been tagged with the commit hash to indicate the version.


#### **Monitor it!**

- Add <INSERT MONITORING TOOL> to the application.
- Create a dashboard to monitor the health of the application.

---

### Prerequisite

Copy the Github repo into your own repository and make it private.

Node v16 is required for this project to run.

We will be using Digital Ocean to host our staging and production environment and our databases. Students get $100 credits which is more than enough to cover our needs.

- [Sign up with Digital Ocean](https://www.digitalocean.com/) and claim [your $100](https://education.github.com/pack)
- Create two droplets in Digital Ocean (pick the cheapest). Name one Staging and the other Production.
- Create two PostgresSQL databases. Make sure to add Staging and Production somewhere to the name of them.

#### Setup your dev environment

Easiest is to use postgres running in a docker container. Create a script that will start a local postgres database running in a docker container.

### Helpful Commands

Run the following commands to get started:

`npm install`

`npm run prisma:init` 

`npm run dev`


## Hand in

Add me (arnif) as collaborator to the repository. Also make sure to send the link in Canvas when handing in the assignment.



Good luck and Have fun :)
