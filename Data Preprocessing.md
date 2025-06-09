Dataset Gaming Effect on Students and Academic Result(no.3)

<table>
  <tr>
    <td></td>
    <td>how much time spending on gaming</td>
    <td>when do you play game the most</td>
    <td>do feel hamper in sleep</td>
    <td>do you feel mental stress</td>
    <td>do you feel depression</td>
  </tr>
  <tr>
    <td>range from raw dataset</td>
    <td> <2 hours <br>3-4 hours <br> >5 hours</td>
    <td>Morning<br>Afternoon<br>Evening<br>Mid-night</td>
    <td>Yes<br>Sometimes<br>No</td>
    <td>Yes<br>Sometimes<br>No</td>
    <td>Yes<br>Sometimes<br>No</td>
  </tr>
  <tr>
    <td>range for classification (split)</td>
    <td>intensity(scoring)<br> <2 hours: low(0)<br> 3-4 hours:average(0.5)<br> >5 hours:high(1)</td>
    <td>scoring<br>Afternoon:0<br>Evening:0.5<br>Mid-night:1</td>
    <td>scoring<br>Yes: 1<br>Sometimes: 0.5<br>No: 0</td>
    <td>scoring<br>Yes: 1<br>Sometimes: 0.5<br>No: 0</td>
    <td>scoring<br>Yes: 1<br>Sometimes: 0.5<br>No: 0</td>
  </tr>
  <tr>
    <td>Classification</td>
    <td colspan="3">Seriousness=time spend on gaming + when play game + hamper in sleep<br>Weight = 1.5<br>Classification: seriousness x weight</td>
    <td colspan="2">Seriousness=mental stress score + depression score<br>Weight = 2<br>Classification: seriousness x weight</td>
  </tr>
</table>



Dataset Student Gaming and Sleep Habit (no.1)

|         | when do you go to sleep| do you feel fatigue | how you feel when you cannot play the in a day|
|--|--|--|--|
| range from raw dataset  |      |    |
| range for classification (split) |    |    |


