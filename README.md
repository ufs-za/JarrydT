# Purchase Intention Prediction App

This application predicts a customer’s intent to purchase based on several different factors, including customer experience ratings and demographic information. The prediction is conducted using a pre-trained **Random Forest** model, which generates predictions based on user inputs. 

## How It Works

Users are asked to provide their inputs such as their customer type and experience ratings. After submitting the inputs by clicking the **Predict Purchase Intention** button, the app displays the predicted **Purchase Intention Level** on a scale from 1 to 5, where:
- **1** indicates very low purchase intention
- **5** indicates very high purchase intention

The app provides the final prediction of the customers intent to purchase as well as a confidence score, reflecting the model's confidence in the prediction. Furthermore, the app allows for multiple predictions by adjusting inputs and resubmitting and allows users to submit feedback on the prediction and overall experience.

## Key Features

- **Interactive Input Form:** Users can enter values through sliders and radio buttons.
- **Prediction Generation:** The app calculates and displays the Purchase Intention level with a confidence percentage.
- **Feedback Portal:** Users are able to provide feedback on the predictions directly through the app.

## Development Challenges

- **Alignment Issues:** Streamlit's slider and radio buttons have different default font sizes, causing misalignment in the layout. To address this, sliders were placed in a separate section to maintain a neat appearance and to better readability.
  
- **Deployment:** Deploying the app on Streamlit proved to be a challenge due to permission issues and different package versions. To circumvent these issues, permission had to be granted and packages needed to be downgraded or different packages had to be used to obtain the desired outcome.

- **Model Integration:** Loading the **Random Forest** model from a pickle file proved to be difficult  due to compatibility issues with the `pickle` package. This was resolved by using **pandas** to load the pickle file, ensuring that the **Random Forest** model was able to be used. 

## Process of Deployment 

- **Application Code:** The core logic of the applications code is written in the `app.py` file. The code imports the **Random Forest** model, sets up the buttons and sliders for the user's interaction, and makes predictions based on the input provided. The code also calculates the confidence level of the prediction, displaying the overall accuracy. Additionally, a feedback button allows the user to submit feedback through a dedicated input box.

- **Supporting Files:** Several supporting files were included in the Streamlit app. The `.streamlit` file contains configuration settings for customizing the app's appearance. Other files include an image of the app's icon, and the pre-trained **Random Forest** model, which is used for generating predictions. The `requirements.txt` file lists all the necessary Python packages needed for the app to run on streamlit.

- **Linking Streamlit:** Once the files were uploaded it is a matter of linking streamlit to the Github repository. This was done by creating an account on Streamlit and linking it to the Github page. The repository is then selected and the app is created. 
  
---

For any further information or contributions, feel free to explore the repository or reach out directly.

Application link: https://jarrydt-purchaseintention.streamlit.app/
