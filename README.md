# comp163-personal-portfolio
A personal portfolio- Comp163
# Description:
# Mastery of Chapter 3 data types (strings, lists, tuples, sets, and dictionaries).



# 1. Personal Information (Strings)

full_name = "Fred Wallace"
student_email = "fxwallace@ncat.edu"
hometown = "Watertown, NY"
graduation_semester = "Spring 2029"
major = "Computer Science"


# 2. Academic Data (Lists)

current_courses = ["COMP 163", "MATH 131", "ENG 101", "Comp 121","SPCH 250","GEEN 111"]
completed_courses = ["African American Studies","US History"]
credit_hours = [1, 1, 3, 3, 4, 3]  # credit hours for current courses
gpa_history = [4.0]  # semester GPAs


# 3. Contact Info (Tuples)

emergency_contact = ("Mom", "Terri Wallace", "910-261-5223")
home_address = ("1112 Shebly PL SE", "Atlanta, GA", "28202")
instagram_info = ("Instagram", "@_.fred_x", 312)
twitter_info = ("Twitter", "@N/A", 127)
birthday = ("Birthday", 8, 22, 2007)


# 4. Interests (Sets)

current_skills = {"Python basics", , "Problem solving", "Time management", "Photography"}
skills_to_learn = {"JavaScript", "Data structures", "Git", "Web design", "Public speaking"}
career_interests = {"Software development", "Web development", "Game development"}
hobbies = {"Gaming", "Photography", "Soccer", "Music"}
entertainment_backlog = {"One Piece", "Naruto"}


# 5. Organizational Mapping

course_credits = {"COMP 163": 3, "MATH 131": 4, "ENG 100": 3, "SPCH 250": 3,"COMP 121": 1, "GEEN 111":1}
course_professors = {"COMP 163": "Prof. Rhodes", "MATH 131": "Prof. Terkper", "ENG 101": "Prof. S.Rhodes", "SPCH 250": "Prof.Chavis","COMP 121": "Prof. Rhodes","GEEN 111": "Prof. Parrish"}
course_rooms = {"COMP 163": "M-Eric 300", "MATH 131": "Crobsy 106","ENG 101": "Merrick 327", "SPCH 250": "Online","COMP 121":Graham 210,"GEEN 111":"McNair 240"}
monthly_budget = {"Food": 450, "Entertainment": 200, "Books": 125, "Transportation": 100}
study_hours = {"Programming": 10, "Math": 8, "English": 4, "Other": 3}
contact_directory = {"Mom": "910-261-5223", "Academic Advisor": "mojones@ncat.edu"}


# 6. Required Calculations

total_credits = credit_hours[0] + credit_hours[1] + credit_hours[2] + credit_hours[3] + credit_hours[4]+credit_hours[5]

cumulative_gpa = (credit_hours[0] + credit_hours[1] + credit_hours[2] + credit_hours[3] + credit_hours[4]+credit_hours[5]) / 4

total_courses=len(current_courses)

completed_count = len(completed_courses)

total_study_hours = study_hours["Programming"] + study_hours["Math"] + study_hours["English"] + study_hours["Other"]

academic_load = total_credits + total_study_hours

monthly_total = monthly_budget["Food"] + monthly_budget["Entertainment"] + monthly_budget["Books"] + monthly_budget["Transportation"]

daily_food_budget = monthly_budget["Food"] / 30

annual_budget = monthly_total * 12

study_cost_per_hour = monthly_budget["Books"] / total_study_hours


# 7. Analytics Calculations

total_followers = instagram_info[2] + twitter_info[2]
skills_comparison = f"{len(current_skills)} current vs {len(skills_to_learn)} learning goals"
contact_count = len(contact_directory)
backlog_count = len(entertainment_backlog)
workload_assessment = f"Credits: {total_credits}, Study Hours: {total_study_hours}"


# Output Display
print("================================================================")
print("              PERSONAL ACADEMIC & LIFE PORTFOLIO")
print("================================================================")
print(f"Student: {full_name} | Email: {student_email}")
print(f"From: {hometown} | Graduating: {graduation_semester}")
print(f"Major: {major}")

print("\n=== ACADEMIC PROFILE ===")
print(f"Current Semester: {total_credits} credits across {total_courses} courses")
print(f"Cumulative GPA: {cumulative_gpa:.2f}")
print(f"Weekly Study Time: {total_study_hours} hours")
print(f"Academic Investment: ${study_cost_per_hour:.1f} per study hour")

print("\nCurrent Courses:")
print(f"{current_courses[0]} - {course_credits['COMP 163']} credits - {course_professors['COMP 163']} - {course_rooms['COMP 163']}")
print(f"{current_courses[1]} - {course_credits['MATH 150']} credits - {course_professors['MATH 150']} - {course_rooms['MATH 150']}")
print(f"{current_courses[2]} - {course_credits['ENG 100']} credits - {course_professors['ENG 100']} - {course_rooms['ENG 100']}")
print(f"{current_courses[3]} - {course_credits['SPCH 250']} credits - {course_professors['SPCH 250']} - {course_rooms['SPCH 250']}")
print(f"{current_courses[3]} - {course_credits['COMP 121']} credits - {course_professors['COMP 121']} - {course_rooms['COMP 121']}")
print(f"{current_courses[3]} - {course_credits['GEEN 111']} credits - {course_professors['GEEN 111']} - {course_rooms['GEEN 111']}")


print("\n=== PERSONAL DEVELOPMENT ===")
print(f"Current Skills: {current_skills}")
print(f"Learning Goals: {skills_to_learn}")
print(f"Career Interests: {career_interests}")
print(f"Skills Currently Have: {len(current_skills)}")
print(f"Skills Want to Learn: {len(skills_to_learn)}")

print("\n=== FINANCIAL OVERVIEW ===")
print(f"Monthly Budget: ${monthly_total}")
print(f"Food: ${monthly_budget['Food']} (${monthly_budget['Food'] / 30}/day)")
print(f"Entertainment: ${monthly_budget['Entertainment']}")
print(f"Books: ${monthly_budget['Books']}")
print(f"Transportation: ${monthly_budget['Transportation']}")
print(f"Annual Projection: ${annual_budget}")

print("\n=== CONNECTIONS & CONTACTS ===")
print(f"Emergency Contact: {emergency_contact[1]} ({emergency_contact[0]}) - {emergency_contact[2]}")
print(f"Home Address: {home_address[0]}, {home_address[1]} {home_address[2]}")
print(f"Social Media Presence: {total_followers} followers across 2 platforms")
print(f"Key Contacts: {contact_count} people in directory")

print("\n=== LIFE STATISTICS ===")
print(f"Total Courses Completed: {completed_count}")
print(f"Current Academic Load: {academic_load} weekly commitments")
print(f"Entertainment Backlog: {backlog_count} items")
print(f"Current Hobbies: {len(hobbies)} activities")
print("================================================================")
