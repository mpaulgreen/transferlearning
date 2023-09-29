- Execution
```
python3 log_model.py
mlflow models serve -m <<path to model>> -p 1234
curl -X POST http://127.0.0.1:1234/invocations -H 'Content-Type:application/json' -d '{"dataframe_split": {"columns": ["text"],"data": [["Today is a perfect day to practice automation skills"]]}     }'
```