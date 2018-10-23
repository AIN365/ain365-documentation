#### AIN365

## Exercise 7 - Validate your dashboard

This exercise is optional.

You will tweet on a predefined hashtag (e.g. #SAPTechEd) and prove that the Twitter dashboard is working as expected.
<br><br>
![](screens/exercise7-0.png)<br><br>
The planned duration for this exercise is 5 minutes. You can find a recording of the exercise [here](https://youtu.be/SyN_LxUnmQc).<br><br><br>

## Steps

Run the following steps to complete the exercise:<br><br>

In the AIN365 dashboard there's no **Geo Location** for **Barcelona, Spain** at the moment.<br><br>
![](screens/exercise7-1.png)<br><br>
Switch to **Twitter** and create a new tweet, e.g. with the text `I'm attending session #AIN365 on #SAPTechEd. I love it :-)` [1] and a custom Geo Location [2]. As an example **Barcelona, Spain** [3] is used here. Afterwards click on **Tweet**.<br><br>
![](screens/exercise7-2.png)<br><br>
Navigate back to your story and click **Refresh**.<br><br>
![](screens/exercise7-3-1.png)<br><br>
You should see at least one new Tweet with a **Geo Location** for the location you used in your Tweet (e.g. Barcelona, Spain). (Note: it might take up to one minute, until your Tweet can be displayed on the dashboard.)<br><br>
![](screens/exercise7-3.png)<br><br>
Click on **Input Variables** and select **AIN365_TRENDINGHASHTAGS**.<br><br>
![](screens/exercise7-4.png)<br><br>
Change the **Time Frame** to **Last 24 Hours**.<br><br>
![](screens/exercise7-5.png)<br><br>
You can now see the **Tweets** for the **Last 24 Hours**. Also the time frames change from **Day** to a range of **6 hours**.<br><br>
![](screens/exercise7-6.png)<br><br>
Click again on **Input Variables** and select **AIN365_TRENDINGHASHTAGS**.<br><br>
![](screens/exercise7-7-1.png)<br><br>
Select **Last 7 Days** for **Time Frame** [1] and any value you like, e.g. **#ain365** or #analytics as **Hashtag** [2]. Afterwards click on **Set**.<br><br>
![](screens/exercise7-7.png)<br><br>
You can see the **Last 7 Days** with all tweets containing **#ain365** in the dashboard.<br><br>
![](screens/exercise7-8.png)<br><br>
Click once more on **Input Variables** and select **AIN365_TRENDINGHASHTAGS**. Select **Show All** for **Time Frame** and confirm with **Set**.<br><br>
![](screens/exercise7-9.png)<br><br>
Select the **Geo Map**, click on the **Map Control** navigation and select the **Polygon Filter** [1]. Choose the **Square** filter [2].<br><br>
![](screens/exercise7-10.png)<br><br>
Mark the area you want to filter for, e.g. here on Europe. Afterwards click the **Filter** icon.<br><br>
![](screens/exercise7-11.png)<br><br>
You can see the **Tweets** filtered by **Geo Location**.<br><br>
![](screens/exercise7-12.png)<br><br>


**Congratulations! You have successfully completed the seventh exercise.**<br><br><br>

## Next Steps
Continue with [Exercise 8](../exercise8/README.md) and create a R visualization.
<br><br><br>


## License

This project is licensed under the SAP SAMPLE CODE LICENSE AGREEMENT except as noted otherwise in the [LICENSE file](../LICENSE).
