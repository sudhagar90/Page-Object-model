# Page-Object-model
Hari - PoM codes

using OpenQA.Selenium;
using OpenQA.Selenium.Chrome;
using System;
namespace FirstSel;
class ProgramSel
{

    static void Main(String[] args)
    {
        // launch browser
        IWebDriver driver = new ChromeDriver();
    

        // Navigate to url
        driver.Navigate().GoToUrl("https://www.google.co.in/");

        // inspect the webelement
        IWebElement element = driver.FindElement(By.Name("q"));

        // perform operation

        element.SendKeys("Wikipedia");


    }



}






