<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>JS</title>
        <style>
           div{
            background:rgb(95, 198, 226);
            text-align:center;
            width:300px;
            margin:auto;
           } 

        </style>
        </head>
        <body>
            <div>
            <h2>Marks Report</h2>
            <table align="center">
                <tr>
                    <td><label>RollNon</label></td>
                    <td><input type="text" id="rno" name="rno"/></td>
                </tr>
                <tr>
                    <td><label>stu Name</label></td>
                    <td><input type="text" id="sna" name="sna"/></td>
                </tr>
                <tr>
                   <td><label>HTML</label></td>
                   <td><input type="text" id="hm" name="hm"/>
                </tr>
                <tr>
                    <td><label>CSS</label></td>
                    <td><input type="text" id="cm" name="cm"/>
                </tr>
                <tr>
                    <td><label>JavaScript</label></td>
                    <td><input type="text" id="jm" name="jm"/>
                </tr>
                <tr  align="center">
                  <td colspan="2"><button onclick="getResult()">get result</button></td>
                </tr>
                <tr  align="center">
                    <td colspan="2"><output id="total"></output> <br>
                        <output id="average"></output>
                </td>
                </tr>
            </table>
            </div>
            <script>
                function getResult()
                {
                  let h,c,j,tot,avg;
                  h = parseInt(hm.value);
                  c = parseInt(cm.valu);
                  j = parseInt(jm.value);
                  tot=h+c+j;
                  avg=tot/3;
                  total.value="Total Marks:"+tot;
                  average.value="Average:"+avg;
                }
            </script>
        </body>
    </head>
</html>
