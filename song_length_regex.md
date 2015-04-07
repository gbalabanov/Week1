import re
match = re.compile(r"^(\d{1,3}:)?(\d{1,2})?(:\d{1,2})$")
length = re.findall(match, "2:32")
print(length)
