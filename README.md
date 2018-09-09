*** Settings ***
Library           Selenium2Library

*** Variables ***
${url}            https://hotline.ua/

*** Test Cases ***
Test Case1
    Open Browser    ${url}    Chrome
    Input Text    searchbox    iPhone 7
    Click Button    doSearch

Test Case2
    Go To    ${url}
    Close Browser
