#The program calculates the cost of a parcel a courier company delivers

distance = input("Enter the total distance of the delivery in kilometres:")

#air freight = print(0.36* float(distance))

#land freight 0.25*float(distance)

#The user is required to choose shipping preference to determine the cost of freight
freight = input("Choose shipping preference: Air or Land")

freight_cost =0
if freight== "Air":
 freight_cost = (float(0.36)*float(distance))
elif freight == "Land":
  freight_cost = (float(0.25)*float(distance))
 #The user is required to choose the type of insurance to determine the cost of insurance
insurance = input("Choose type of insurance:Full insurance or limited insurance")

insurance_cost =0
if insurance == "Full insurance":
 insurance_cost = 50.00
elif insurance== "limited insurance":
 insurance_cost = 25.00
#The user is required to choose if they want to add a gift to determine the cost of gift
gift = input("Add gift?:Yes or No")

gift_cost=0
if gift =="Yes":
 gift_cost =15.00
elif gift == "No":
 gift_cost =0.00
#The user is required to choose the type of delivery to determine the cost of delivery method
priority = input("Choose type of delivery: Priority delivery or Standard delivery")

priority_cost =0
if priority == "Priority delivery":
 priority_cost = 100.00
elif priority == "Standard delivery":
 priority_cost = 20.00
#The user is required to choose parcel option to determine the cost of parcel 
parcel = input("Choose parcel option: Postage sleeve or Postage box")

parcel_cost =0
if parcel == "Postage sleeve":
 parcel_cost= 100.00
elif parcel == "Postage box":
 parcel_cost= 150.00
 
total_cost = freight_cost + insurance_cost + gift_cost + priority_cost + parcel_cost
print(f"The cost of sending a parcel is R{total_cost}.")
