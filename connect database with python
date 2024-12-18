import pymysql

# database connection
connection = pymysql.connect(host="localhost", port=3306, user="root", passwd="tm123789", database="CompanyDB")
cursor = connection.cursor()
# some other statements  with the help of cursor

print("Connection Established")

empId=input("Please enter an employeeID")

cursor.execute("SELECT * FROM Employees Where employee_id="+empId)

myresult = cursor.fetchall()

for x in myresult:
  print(x)

connection.close()
