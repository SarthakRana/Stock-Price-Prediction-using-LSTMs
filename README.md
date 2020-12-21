# 💸 Stock Price Forecasting using LSTMs 📈

### Try out the project here -- https://stock-price-forecasting.herokuapp.com/
*(Please wait for 12-15 seconds for app to load initially)*
<br><br>

![](https://www.thebalance.com/thmb/nQn7Hs8wx2wqUwC7h-TT1xrnJWo=/4608x2592/filters:fill(auto,1)/close-up-of-chart-on-digital-display-887362798-5a65990b0d327a0036c0ea79.jpg)

<br><br>
This is a Stock Price Forecasting project wherein I have used an LSTM based model trained on previous 10 years of Apple's Closing stock prices. The model is capable of forecasting next 1, 2 and 3 days of closing stock price.

## 1. Prerequisites

You need to have the following dependecies before running the project:

- pandas `pip install pandas`
- numpy `pip install numpy`
- scipy `pip install scipy`
- scikit learn `pip install scikit-learn`
- streamlit `pip install streamlit`
- matplotlib `pip install matplotlib`
- seaborn `pip install seaborn`
- tensorflow `pip install tensorflow`
- pandas datareader `pip install pandas-datareader`

## 2. Installing

Use the package manager to install __Stock Price Forecasting using LSTMs__ project

You can clone the repo :
```
gitclone https://github.com/SarthakRana/Stock-Price-Prediction-using-LSTMs.git
```

GitHub CLI :
```
gh repo clone SarthakRana/Stock-Price-Prediction-using-LSTMs
```

You can also download the ZIP of this project and place on your working directory.

## 3. Usage

### 3.1 Web App

1. Install all dependencies mentioned in __Prerequisites__.
2. Open CLI/prompt and make sure Streamlit is installed by running the command `streamlit --version`. You should see something like this : `Streamlit, version 0.67.1`.
3. Do this for all other dependencies as well just to make sure everything is in right place and you are good to go.
4. Go to your working directory(where you have placed the .py file and other components) and open CLI/prompt there.
5. Type in the following command and press Enter :<br>
   `streamlit run app.py`<br>
   Please wait for 5-10 seconds for command to run.
6. A browser widow should open up with the app running.
7. Enjoy :)

### 3.2 Project

1. Install all dependencies mentioned in __Prerequisites__.
2. Place the contents of project folder in your working directory.
3. Simply open Jupyter Notebooks/Jupyter Lab and run the .ipynb files.
4. All project related files like models, scalers and encoders will be saved in the same directory as you run the files.

## 4. Deployment

For deployment on Heroku, we need to make 3 extra files.

### 4.1 Procfile

Create a procfile and copy the below code :
```
web: sh setup.sh && streamlit run app.py
```
### 4.2 requirements.txt

Run the below command to prepare the requirements.txt

```
pip freeze > requirements.txt
```

NOTE : I personally don't use the freeeze command as it creates some version conflicts while deploying on Heroku. I prefer writing doing the required packages name in the txt file. Heroku automatically makes use of the latest package version available while deploying.

### 4.3 setup.sh

Create a file `setup.sh` and copy the below code:

```
mkdir -p ~/.streamlit/
echo "\
[general]\n\
email = \"your-email@domain.com\"\n\
" > ~/.streamlit/credentials.toml
echo "\
[server]\n\
headless = true\n\
enableCORS=false\n\
port = $PORT\n\
" > ~/.streamlit/config.toml
```

### 4.4 Full deployment

NOTE : To deploy on Heroku, you can either use Heroku CLI or Heroku Dashboard.
You can follow the rest of the steps from here : https://www.youtube.com/watch?v=IWWu9M-aisA

## 5. Roadmap

See the open issues for a list of proposed features (and known issues)(if any).
If your issue is not listed in the already open issues, you can open up a new one.

## 6. To-do

- [ ] Add stock tickers for Amazon, Tesla, Google, HDFC Bank, etc.
- [ ] Add EDA for each stock ticker on a separate web page.

## 7. Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are greatly appreciated.

  1. Fork the Project.
  2. Create your Feature Branch.
  3. Commit your Changes.
  4. Push to the Branch.
  5. Open a Pull Request.

## 8. Authors

NOTE : Your name will be added here if I merge your pull request.

Sarthak Rana (https://www.linkedin.com/in/sarthakrana/)
