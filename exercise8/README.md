#### AIN365

## Exercise 8 - Extend with R Visualization
This exercise is optional.

You will use the extracted hashtags from the AIN365 core application and integrate a R visualization on the HANA 2.0 Live Connection (word cloud).
<br><br>
![](screens/exercise8-0.png)<br><br>
The planned duration for this exercise is 10 minutes. You can find a recording of the exercise [here](https://youtu.be/g4_SJeOr71s).<br><br><br>

## Steps

Run the following steps to complete the exercise:<br><br>

Open the **Menu** bar and select **Create** > **Model**.<br><br>
![](screens/exercise8-1.png)<br><br>
Choose **Get data from a datasource** [1] and select **Live Data connection** [2].<br><br>
![](screens/exercise8-2.png)<br><br>
Select **SAP HANA** as **System Type** [1], **AIN365CF** as **Connection** [2] and **trendingHashtags** as **Data Source** [3]. Afterwards name the model **USERID_TRENDINGHASHTAGS** [4] (e.g. USERXX_TRENDINGHASHTAGS) and add **CV trendingHashtags** as **Description** [5]. Finally click on **OK**.<br><br>
![](screens/exercise8-4.png)<br><br>
Keep the default settings and click **Save**.<br><br>
![](screens/exercise8-5.png)<br><br>
Navigate back to your story via **Menu Bar** > **Browse** > **Files** and select your story.<br><br>
Switch to the tab **Tweets II (Live)** and click on the **Plus** [1] sign to add a **R Visualization** [2].<br><br>

> **NOTE**
>
> Once your SAP Analytics Cloud tab is too small (resolution), the **Plus** [1] icon will move to the **More** section (... icon).

<br>

![](screens/exercise8-6.png)<br><br>
Mark the **R Visualization** [1] and click in the **Designer** on **Add Input Data** [2].<br><br>
![](screens/exercise8-7.png)<br><br>
Click on the **Change** icon to select the newly created model.<br><br>
![](screens/exercise8-8.png)<br><br>
Confirm the warning message while changing the model.<br><br>
![](screens/exercise8-9.png)<br><br>
Select your model, e.g. **USER01_TRENDINGHASHTAGS** and click on **OK**.<br><br>
![](screens/exercise8-10.png)<br><br>
Change the **Time Frame** [1] to **Last 7 Days** and confirm the settings with **Set**.<br><br>
![](screens/exercise8-11.png)<br><br>
Click on **Add Dimensions** [1] in the **Rows** section, select **HASHTAG** [2] and click **OK** on the bottom right.<br><br>
![](screens/exercise8-12.png)<br><br>
You should see the model selected (e.g. USERXX_TRENDINGHASHTAGS) containing 1 Measure and 1 Dimension [1].<br><br>
Click on the **Add Script** [2] link.<br><br>
![](screens/exercise8-13.png)<br><br>
Click on the **Expand** screen to maximize the screen.<br><br>
![](screens/exercise8-14-1.png)<br><br>
Copy & Paste the [snippet](../misc/wordcloud.txt) to the **Editor**.<br><br>
![](screens/exercise8-14.png)<br><br>
Adjust the required parameters to your input model.<br><br>
Therefore change
- **YOUR_MODEL_NAME** [1] to your user, e.g. **USERXX_TRENDINGHASHTAGS**,
- **HASHTAG_TO_FILTER** [2] to **#SAPTECHED**,
- **data$HASHTAG_DIMENSION** [3] to **data$Hashtag** and
- **data$HASHTAG_MEASURE** [4] to **data$\`No. of Entries\`**.

Afterwards click **Execute** to preview or click directly on **Apply** to close the **editor**.<br><br>
![](screens/exercise8-15.png)<br><br>
Select the **R Visualization** [1], click on **More Actions** (...) > **Show / Hide** and disable all properties [2].<br><br>
![](screens/exercise8-16.png)<br><br>
The **word cloud** has been rendered using R Serve.<br><br>
In addition it's possible to link the input parameters with the one's from the other models within our story.<br><br>
![](screens/exercise8-17.png)<br><br>
Switch back to the **Editor** (**Edit Script** on the **Designer**). Change e.g. the **min.freq** of the words from **5** to **2** and play around with it. Afterwards confirm with **Apply**.<br><br>
![](screens/exercise8-18.png)<br><br>
You will find more **hashtags** on the visualization now.<br><br>
![](screens/exercise8-19.png)<br><br>


**Congratulations! You have successfully completed the eighth exercise.**<br><br><br>
**Congratulations! You have successfully completed all exercises of this TechEd session!**<br><br><br>


## License

This project is licensed under the SAP SAMPLE CODE LICENSE AGREEMENT except as noted otherwise in the [LICENSE file](../LICENSE).
