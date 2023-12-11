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

#### Step 2: Run the Backend Server

In your terminal, run the following command to start the backend server:

```bash
cd bss-server/bssBack
/* 이곳에 서버 빌드하는 명령어 입력 필요 */
```

#### Step 3: Install Frontend Dependencies
Open a new terminal window, and run the following command to install the frontend dependencies:

```bash
cd bss-client
```

```bash
npm install
```

#### Step 4: Check the Environment File

- Check a file named `.env.local` in the `bss-main/bss-client` directory.
> This file will store the environment variable for the project to run.

#### Step 5: Run the Frontend Server

After installing the frontend dependencies and checking the environment file, run the following command in the same terminal to start the frontend server:

```bash
npm run dev
```

This command will start the frontend server, and you'll be able to access the website on `localhost:3000` in your web browser.
