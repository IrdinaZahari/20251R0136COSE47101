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



Dataset uniGame (no.1)

<table>
  <tr>
    <td></td>
    <td>Your current GPA</td>
    <td>when you go to sleep </td>
    <td>do you attend your morning class regularly</td>
    <td>avg time spend on playing games</td>
    <td>how many time you spend with family and friends</td>
    <td>do you feel fatigue</td>
  </tr>
  <tr>
    <td>range from raw dataset</td>
    <td>minimum: 2<br>maximum: 4</td>
    <td>10 distinct times:<br>0<br>1<br>2<br>3<br>4<br>5<br>7<br>8<br>22<br>23</td>
    <td>Yes<br>No</td>
    <td>9 distinct values:<br>0<br>1<br>2<br>3<br>4<br>5<br>6<br>7<br>8</td>
    <td>8 distinct values:<br>0<br>1<br>2<br>3<br>4<br>5<br>6<br>7</td>
    <td>Yes<br>No</td>
  </tr>
  <tr>
    <td>range for classification (split)</td>
    <td>2.00-2.49: low(3)<br>2.50-2.99: average(2)<br>3.00-3.49: good(1)(<br>3.50-4.00: excellent(0)</td>
    <td>20,21,22: healthy(0)<br>23,0,1: average(1)<br>2,3,4: late (2)<br>5,6,7,8: very late (3)</td>
    <td>Yes(0)<br>No(1)</td>
    <td>0-2hrs: low(0)<br>3-5hrs: moderate(1)<br>6+hrs: high(2)</td>
    <td>0-2hrs: low(2)<br>3-5hrs: moderate(1)<br>6+hrs: high(0)</td>
    <td>Yes(1)<br>No(0)</td>
  </tr>
  <tr>
    <td>Deciding label</td>
    <td colspan="6">*Add score of all attribute<br>Need time management?<br> 0-5: No<br> 6-12: Yes</td>
  </tr>
</table>




