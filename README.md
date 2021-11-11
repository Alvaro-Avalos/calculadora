# calculadora
my first repository
//the example is written in MS Coded UI using c# language.
[TestMethod]
public void TestCalculator()
{
 
//launch the application
var app = ApplicationUnderTest.Launch("C:\\Windows\\System32\\calc.exe");
 
//do all the operations
Mouse.Click(button2);
Mouse.Click(buttonAdd);
Mouse.Click(button3);
Mouse.Click(buttonEqual);
 
//evaluate the results
Assert.AreEqual("5", txtResult.DisplayText,”Calculator is not showing 5);
 
//close the application
app.Close();
}
