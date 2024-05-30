# Deploying the [Python] Shiny App

## Resources: 

* https://docs.posit.co/shinyapps.io/guide/getting_started/index.html#working-with-shiny-for-python

## Workflow

1. Install rsconnect-python: `pip install rsconnect-python`

2. Configure rsconnect-python [link](https://docs.posit.co/shinyapps.io/guide/getting_started/index.html#configure-rsconnect-python)

   * Retrieve the token code
   * Run it in the Python command prompt

3. Deploy the app  
   ```bash
   rsconnect deploy shiny C:\Workspace\ARCCCOH\SurveillanceDashboard\src --name johnpfay --title Case-LDAS-correlations
   ```

   

   