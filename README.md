# din folderul sales_analysis
git init
git add .
git commit -m "Added initial sales analysis project scaffold."
git branch -M main
git remote add origin https://github.com/<user>/sales_analysis.git
git push -u origin main
git checkout -b analyze-sales
# Deschide sales_data.py și adaugă funcțiile + apelurile lor
# (poți lua exemplul din README.md)

git add sales_data.py
git commit -m "Implemented total and average sales functions."
git push -u origin analyze-sales
git checkout main
# Editează sales_data.py: păstrează varianta simplă + adaugă comentariul:
# Weekly sales data: [Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday]

git add sales_data.py
git commit -m "Added comment explaining sales_data list structure."
git pushgit merge analyze-sales
# vei vedea <<<<<<< HEAD / ======= / >>>>>>> analyze-sales în sales_data.py
# Rezolvă manual:
# - păstrează comentariul explicativ
# - păstrează funcțiile total_sales și average_sales
# - păstrează apelurile funcțiilor din blocul if __name__ == "__main__":

# Exemplu final corect:
# sales_data.py
#
# Weekly sales data: [Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday]
# sales_data = [...]
# def total_sales(...):
# def average_sales(...):
# if __name__ == "__main__": ...

git add sales_data.py
git commit -m "Resolved conflicts and merged analyze-sales into main."
git push

