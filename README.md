# Tabpy Forecasting
Use of Tabpy to access data and create GUI for user with backend supporting a python-based SARIMAX forecasting model.

Tabpy Setup Process:
 * From your preferred Python IDE create a new project with the use of a virtual environment.
 * Within your Python IDE open the terminal and execute the following commands in the order listed below.
    * pip install --upgrade pip
    * pip install tabpy
    * tabpy
 * Upon running "tabpy" in the terminal local port 9004 will be opened and made available to connect to from Tableau
 * Within your virtual environment navigate to the following file path to extend the timeout threshold from 30 seconds to 10 minutes
    * /env/lib/python3.8/site-packages/tabpy/tabpy_server/app/app.py
 * Navigate to Tableau and select; Help -> Settings and Performance -> "Manage Analytics Extensions Connection" and set "Hostname" = "localhost" and "Port" = 9004
 * Select "Test Connection" to confirm connection has been made
 * Once confirmed select "Save" and then "Close" 
