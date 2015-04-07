import re
match = re.compile(r"^(\d{1,3})?:?(\d{1,2})?:?(\d{1,2})$")

for x in match.search("2:32:3").groups():
    print(int(x))
