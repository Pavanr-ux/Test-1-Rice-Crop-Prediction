# Rice Crop Prediction

## Project Overview
This project aims to develop a regression model using a *Random Forest Regressor* algorithm. Key metrics employed for evaluating the model's performance include R², MAE (Mean Absolute Error), and MSE (Mean Squared Error).

## Project Structure

### Files
1. **app.py**: Contains the regression model code.
2. **requirements.txt**: Lists all required libraries.
3. **Liver Patient Dataset (LPD)_train.csv**: Dataset with consumer forecast data.
4. **Dockerfile**: Instructions to containerize the application using Docker.
5. **selenium_test.py**: Automated testing using Selenium.
6. **templates/index.html**: HTML file used for rendering the content generated by `app.py`.

### Key Commands

#### Git & CLI
1. **Create a folder**: `mkdir <file_name>`
2. **Navigate to the folder**: `cd <file_name>`
3. **Initialize as Git repository**: `git init`
4. **Add files manually**, then use `git add .` to stage all files.
5. **Commit staged files**: `git commit -m "<message>"`
6. **Connect GitHub repository**: `git remote add origin <GitHub repository link>`
7. **Push files to GitHub**: `git push --set-upstream origin master`

### CI/CD: Jenkins Integration
1. **Create New Item**: Named **<item_name>**
2. **Project Type**: Selected *Freestyle project*
3. **Source Code Management**: Configured as *Git*
4. **Build Step**: Added *Execute Windows batch command*
5. **Save Configuration** and initiate *Build Now*

   **Sample Output:**
   ![Jenkins Output](https://github.com/user-attachments/assets/ee896205-6fbf-4105-ab0a-e3b5969ac210)

### Containerization: Docker
1. **Path Navigation**: Use `cd` and `cd..` to reach the project directory containing the Dockerfile.
2. **Build Docker Image**: Run `docker build -t <docker_image_name> .`
3. **Run Docker Image**: Execute `docker run <docker_image_name>`

   **Output**:
   
   **Command Prompt:**
   ![Command Prompt Output](https://github.com/user-attachments/assets/77f56cf7-610b-4609-a3e5-2ffaec1c90f8)
   ![Output 3](https://github.com/user-attachments/assets/d3615a52-0f2d-459b-846f-19a4ba21cc85)
   
   **Docker Hub:**
   ![Docker Hub Output](https://github.com/user-attachments/assets/3335af03-867c-48cf-a58e-c70fa48d84e6)

### Automated Testing: Selenium
1. **Flask Integration**: Embedded within `app.py` to render `index.html` for web display.
2. **Selenium Test Setup**: Automated test written in `selenium_test.py` to validate the app functionality.

   **Output**:

   **Flask Application (Command Prompt):**
   ![Flask Command Prompt Output](https://github.com/user-attachments/assets/75b060d7-06f3-4a39-9fda-781939519d69)

   **Flask Application (Web Browser):**
   ![Flask Web Browser Output](https://github.com/user-attachments/assets/34f6ec18-5520-412f-a77d-380d7731803a)

   **Selenium Test Output:**
   ![Selenium Test Output](https://github.com/user-attachments/assets/068a30f5-98cc-48a7-9e57-b081b4573deb)