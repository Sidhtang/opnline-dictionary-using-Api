# opnline-dictionary-using-Api
it is a  simple dictionar using python and APIs
the code is short and precise.
import requests
text=input("enter the word you want to search: ")
url="https://api.dictionaryapi.dev/api/v2/entries/en/"+text
meaning=requests.get(url).json()
txtmeaning=str(meaning[0]['meanings'][0]['definitions'][0]['definition'])
print(txtmeaning)

