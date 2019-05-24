# SentimentAnalysisFunctionsApp
SentimentAnalysisFunctionsApp, deployed by azure function, a demo

# how to test

```
power shell
$Invoke-RestMethod "http://localhost:7071/api/AnalyzeSentiment" -Method Post -Body (@{SentimentText="This is a very bad steak"} | ConvertTo-Json) -ContentType "application/json"

content:
{
    "SentimentText":  "This is a ver\ny bad steak"
}

```