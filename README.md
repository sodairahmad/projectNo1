# projectNo1
        def employee_detail():

            emp_name = input("enter employee name :")
            emp_address = input("enter employee address :")
            emp_age = input("enter employee age :")
            emp_id_no = input("enter employee id no  :")
            emp_idcard_no = input("enter employee id card no : ")
            emp_salary = int(input("enter employee salary : "))
            # self.emp_salary = emp_salary
            choose = input("enter yes for taking allowance or no for not taking allowance")
            if choose == 'yes':
                cho = input("enter e for educ, h for health, ex for experience or spo for sport allowance")
                if cho == 'e':
                    ed_allowance = 2000

                    salary = emp_salary + ed_allowance
                    tax = (salary * 20) / 100
                    net_salary = (salary - tax)
                    print(f"your net salary is {net_salary}  and you have"
                          f" to pay {tax}  tax")
                elif cho == 'h':
                    hel_allowance = 1000
                    salary = emp_salary + hel_allowance
                    tax = (salary * 10) / 100
                    net_salary = (salary - tax)
                    total = net_salary + tax
                    print(f"your net salary is Rs : {net_salary}  and you have to pay Rs {tax} tax  "
                          f" and total money = {total}")
            else:
                print("your net salry is ", emp_salary, " you don't need to pay tax ")
