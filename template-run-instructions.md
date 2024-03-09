# Template installation instructions

Feel free to drop these below template installation instructions into your own project's README and tweak according to your needs.

## Installation

### Fork project to your GitHub account

1. Follow the guide [**here**](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo#forking-a-repository)

### Cloning project to your machine

2. Follow the guide [**here**](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo#cloning-your-forked-repository)

### Open project in VSCode

3. Once the project is on your machine, drag the folder and drop it in VSCode to open it or run the [shortcut](https://www.freecodecamp.org/news/how-to-open-visual-studio-code-from-your-terminal/):

```
cd <path to project directory>
code .
```

### Add DOT env with your DB password

4. Create a .env file at the top level of your project with the following (all other details are already in the model/database.js file)

```
DB_PASS=<your password>
```

### Create DB

5. Open up the terminal in VSCode and run

```
mysql -u root -p
<enter your mysql password>
CREATE DATABASE <db name (it's in the model/database.js file)>;
```

Or if you already have set up mysql so you skip entering password:

```
mysql
CREATE DATABASE <db name (it's in the model/database.js file)>;
```

Don't quit. Leave it be to execute your queries.

### Install backend packages and set up db tables and populate with initial data

5. In a FRESH, second terminal run:

```
npm i
npm run migrate
```

### Start expresss server

6. In the same terminal run:

```
npm start
```

Don't kill it; let it run.

### Install frontend packages and start frontend dev server

7. In a THIRD terminal run:

```
cd client
npm i
npm run dev
```

Don't kill it; let it run.

Fin!
