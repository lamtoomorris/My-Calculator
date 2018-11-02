# My-Calculator<!DOCTYPE <!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>Document</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="cal.css" />
    <script src="cal.js"></script>
</head>
<style>
    body{
        background-color: green
    }
</style>

<body>
    <center>
        <h1>My Calculator</h1>
        <form name="calculator">
            <table bgcolor="#aaaaaa" width=220>
                <tr>
                    <td>
                        <table bgcolor="#cccccc" border=1>
                            <tr>
                                <td>
                                    <table border=0 cellpadding=0>
                                        <tr>
                                            <td bgcolor="#aaaaaa"><b style="color: white">Calculator</b></td>
                                        </tr>
                                        <tr>
                                            <td>
                                                <table width="10%" border=0>
                                                    <tr>
                                                        <td colspan=6><input type="text" name="answer" size=30
                                                                maxlength=30 onChange="CheckNumber(this.value)"></td>
                                                    </tr>
                                                    <tr>
                                                        <td colspan=6>
                                                            <table border=0 cellpadding=0>
                                                                <tr>
                                                                    <td>
                                                                        <input type="text" name="mem" size=3 maxlength=3>
                                                                        <input type="button" name="backspace" class="red"
                                                                            value="Backspace" onClick="Backspace(document.calculator.answer.value); return false;">
                                                                        <input type="button" name="CE" class="red"
                                                                            value=" CE " onClick="CECalc(); return false;">
                                                                        <input type="reset" name="C" class="red" value="  C  "
                                                                            onClick="ClearCalc(); return false;">
                                                                    </td>
                                                                </tr>
                                                            </table>
                                                        </td>
                                                    </tr>
                                                    <tr>
                                                        <td><input type="button" name="MC" class="red" value=" MC "
                                                                onClick="MemoryClear(); return false;"></td>
                                                        <td><input type="button" name="calc7" class="blue" value="  7  "
                                                                onClick="CheckNumber('7'); return false;"></td>
                                                        <td><input type="button" name="calc8" class="blue" value="  8  "
                                                                onClick="CheckNumber('8'); return false;"></td>
                                                        <td><input type="button" name="calc9" class="blue" value="  9  "
                                                                onClick="CheckNumber('9'); return false;"></td>
                                                        <td><input type="button" name="divide" class="red" value="  /  "
                                                                onClick="DivButton(1); return false;"></td>
                                                        <td><input type="button" name="sqrt" class="blue" value="sqrt"
                                                                onClick="SqrtButton(); return false;"></td>
                                                    </tr>
                                                    <tr>
                                                        <td><input type="button" name="MR" class="red" value=" MR "
                                                                onClick="MemoryRecall(Memory); return false;"></td>
                                                        <td><input type="button" name="calc4" class="blue" value="  4  "
                                                                onClick="CheckNumber('4'); return false;"></td>
                                                        <td><input type="button" name="calc5" class="blue" value="  5  "
                                                                onClick="CheckNumber('5'); return false;"></td>
                                                        <td><input type="button" name="calc6" class="blue" value="  6  "
                                                                onClick="CheckNumber('6'); return false;"></td>
                                                        <td><input type="button" name="multiply" class="red" value="  *  "
                                                                onClick="MultButton(1); return false;"></td>
                                                        <td><input type="button" name="percent" class="blue" value=" %  "
                                                                onClick="PercentButton(); return false;"></td>
                                                    </tr>
                                                    <tr>
                                                        <td><input type="button" name="MS" class="red" value=" MS "
                                                                onClick="MemorySubtract

(document.calculator.answer.value); return false;"></td>
                                                        <td><input type="button" name="calc1" class="blue" value="  1  "
                                                                onClick="CheckNumber('1'); return false;"></td>
                                                        <td><input type="button" name="calc2" class="blue" value="  2  "
                                                                onClick="CheckNumber('2'); return false;"></td>
                                                        <td><input type="button" name="calc3" class="blue" value="  3  "
                                                                onClick="CheckNumber('3'); return false;"></td>
                                                        <td><input type="button" name="minus" class="red" value="  -  "
                                                                onClick="SubButton(1); return false;"></td>
                                                        <td><input type="button" name="recip" class="blue" value="1/x "
                                                                onClick="RecipButton(); return false;"></td>
                                                    </tr>
                                                    <tr>
                                                        <td><input type="button" name="Mplus" class="red" value=" M+  "
                                                                onClick="MemoryAdd

(document.calculator.answer.value); return false;"></td>
                                                        <td><input type="button" name="calc0" class="blue" value="  0  "
                                                                onClick="CheckNumber('0'); return false;"></td>
                                                        <td><input type="button" name="negate" class="blue" value="+/- "
                                                                onClick="NegateButton(); return false;"></td>
                                                        <td><input type="button" name="dot" class="blue" value="  .   "
                                                                onClick="CheckNumber('.'); return false;"></td>
                                                        <td><input type="button" name="plus" class="red" value=" +  "
                                                                onClick="AddButton(1); return false;"></td>
                                                        <td><input type="button" name="equal" class="red" value="  =   "
                                                                onClick="EqualButton(); return false;"></td>
                                                    </tr>
                                                </table>
                                            </td>
                                        </tr>
                                    </table>
                                </td>
                            </tr>
                        </table>
                    </td>
                </tr>
            </table>
        </form>
    </center>

</body>

</html>
