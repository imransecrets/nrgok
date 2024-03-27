# NRGOK CONFIGURATION FOR POETRY IN WINDOW

Install ngrok via Chocolatey with the following command:

`poetry add choco install ngrok`

Run the following command to add your authtoken to the default ngrok.yml configuration file.

`poetry run ngrok config add-authtoken 2diq6BIok5BHEqKt2kVYUIU5OWC_55hrUjpvq7uaGJLY3KSAp`

Deploy your app online
Put your app online at ephemeral domain Forwarding to your upstream service. For example, if it is listening on port http://localhost:8000, run:

`poetry run ngrok http http://localhost:8080`

===============================================================================
## for static domain

go to `domain` and click on `+ Create Domain` then domain will be created automatically

go to `edges` and click on `+ Create Edge` then 
    select tab `HTTPS`
    select endpoint `a domain for me`
    click on button `Create Edge`
    
now new window open with Congrats! You've got a spot on the internet.

    now click on button `Start a Tunnel` 
    
    you will be given 3 option dropdown menu
    
      1. Start a Tunnel from Command line `[select this one]`

      2. Start a Tunnel from the Config File
      
      3. Start a Tunnel from Docker
      
    copy and past following like command line
    
    write down poetry run and complete the port in my case extrat 00 
    
    poetry run `ngrok tunnel --label edge=edghts_2eHZu2dY9XIe5pE5ly510oAzYoi http://localhost:80`00
    final command should be below
    
    'poetry run ngrok tunnel --label edge=edghts_2eHZu2dY9XIe5pE5ly510oAzYoi http://localhost:8000'
    

    now click the static domain and it will work
  
      






