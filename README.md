<div align="center">
  <img src="https://github.com/bae-sisi/bss-main/assets/56868605/dcc55dc4-3265-4b48-b582-ba052aff51e3" width="125px" />

  <h1>BaeSisi</h1>
    <p align="center">
        <p>CBNU_SW Academic Information Sharing Website</p>
    </p>
</div>

<br/>

## Getting started

#### Step 1: Clone the repository

```bash
git clone https://github.com/bae-sisi/bss-main.git
```

```bash
cd bss-main/
```

```bash
git clone https://github.com/bae-sisi/bss-server.git
```

```bash
git clone https://github.com/bae-sisi/bss-client.git
```

#### Step 2: Database Setting

1. **Connect to MySQL**: 
   - Open MySQL and connect to the server at `localhost:3306` using the `root` user.

2. **Execute SQL Scripts**: 
   - Navigate to the `bss-server/SQL/Final_SQL` directory.
   - Open the `Final_SQL` file and execute all SQL statements in the order they appear.

3. **Import Database**: 
   - In MySQL, click on `Administration`.
   - Select `Data Import/Restore`.
   - Under `Import from Dump Project Folder`, choose the `bss-server/baesisi_SQL` folder.
   - Click on `Start Import` to import the database.
  
#### Step 3: Backend Setting

1. **Configure Application Properties**: 
   - Go to `src/main/resources/application.properties` in your backend project directory.
   - Locate the line `spring.datasource.password = ENTER_YOUR_PASSWORD`.
   - Replace `ENTER_YOUR_PASSWORD` with your MySQL password.

#### Step 4: Run the Backend Server

In your terminal, run the following command to start the backend server:

```bash
cd bss-server/bssBack
chmod +x gradlew
./gradle build
java -jar ./build/libs/bssBack-0.0.1-SNAPSHOT.jar
```

#### Step 5: Install Frontend Dependencies
Open a new terminal window, and run the following command to install the frontend dependencies:

```bash
cd bss-client
```

```bash
npm install
```

#### Step 6: Check the Environment File

- Check a file named `.env.local` in the `bss-main/bss-client` directory.
> This file will store the environment variable for the project to run.

#### Step 7: Run the Frontend Server

After installing the frontend dependencies and checking the environment file, run the following command in the same terminal to start the frontend server:

```bash
npm run dev
```

This command will start the frontend server, and you'll be able to access the website on `localhost:3000` in your web browser.
