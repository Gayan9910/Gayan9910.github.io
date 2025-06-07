# Sample data
headers = ["Name", "Age", "City"]
rows = [
    ["Alice", 30, "New York"],
    ["Bob", 25, "London"],
    ["Charlie", 35, "Sydney"]
]

# Create Markdown table
md_table = "| " + " | ".join(headers) + " |\n"
md_table += "| " + " | ".join(["---"] * len(headers)) + " |\n"
for row in rows:
    md_table += "| " + " | ".join(map(str, row)) + " |\n"

print(md_table)
