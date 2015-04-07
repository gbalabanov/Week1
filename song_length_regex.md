import re
match = re.search(r"^(\d{1,3})?:?(\d{1,2})?:?(\d{1,2})$","23:2")
print(bool(match))
