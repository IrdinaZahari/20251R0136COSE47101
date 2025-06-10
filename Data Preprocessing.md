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
    <td>scoring<br>Morning:0<br>Afternoon:0<br>Evening:0.5<br>Mid-night:1</td>
    <td>scoring<br>Yes: 1<br>Sometimes: 0.5<br>No: 0</td>
    <td>scoring<br>Yes: 1<br>Sometimes: 0.5<br>No: 0</td>
    <td>scoring<br>Yes: 1<br>Sometimes: 0.5<br>No: 0</td>
  </tr>
  <tr>
    <td>Classification</td>
    <td colspan="3">Seriousness_gaming=time spend on gaming + when play game + hamper in sleep<br>Weight = 1.0<br>Classification: seriousness x weight</td>
    <td colspan="2">Seriousness_mental=mental stress score + depression score<br>Weight = 1.5<br>Classification: seriousness x weight</td>
  </tr>
</table>



Dataset Student Gaming and Sleep Habit (no.1)

<table>
  <tr>
    <td></td>
    <td>Your current GPA</td>
    <td>when you go to sleep</td>
    <td>do you attend your morning class regularly</td>
    <td>how many time you spend with family and friends</td>
    <td>do you feel fatigue</td>
  </tr>
  <tr>
    <td>range from raw dataset</td>
    <td> <2 hours <br>3-4 hours <br> >5 hours</td>
    <td>Morning<br>Afternoon<br>Evening<br>Mid-night</td>
    <td>Yes<br>No</td>
    <td>Yes<br>Sometimes<br>No</td>
    <td>Yes<br>No</td>
  </tr>
  <tr>
    <td>range for classification (split)</td>
    <td>intensity(scoring)<br> <2 hours: low(0)<br> 3-4 hours:average(0.5)<br> >5 hours:high(1)</td>
    <td>scoring<br>Morning:0<br>Afternoon:0<br>Evening:0.5<br>Mid-night:1</td>
    <td>scoring<br>Yes: 1<br>Sometimes: 0.5<br>No: 0</td>
    <td>scoring<br>Yes: 1<br>Sometimes: 0.5<br>No: 0</td>
    <td>scoring<br>Yes: 1<br>Sometimes: 0.5<br>No: 0</td>
  </tr>
  <tr>
    <td>Classification</td>
    <td colspan="3">Seriousness_gaming=time spend on gaming + when play game + hamper in sleep<br>Weight = 1.0<br>Classification: seriousness x weight</td>
    <td colspan="2">Seriousness_mental=mental stress score + depression score<br>Weight = 1.5<br>Classification: seriousness x weight</td>
  </tr>
</table>




