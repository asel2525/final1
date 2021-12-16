Endpoints

1. Doctor:

    api/v1/doctor/registration/
    api/v1/doctor/login/
    api/v1/doctor/profile/
    api/v1/doctor/appointments/

2. Patient:

    api/v1/pet/registration/
    api/v1/pet/login/
    api/v1/pet/profile/
    api/v1/pet/history/
    api/v1/pet/appointment/
    
 
POST api/doctor/registration/

Details: API endpoint for creating new doctor account.

request body:

{
    "user_data": {
        "username": "doctor1",
        "first_name": "Dr. Deal",
        "last_name": "Walker",
        "password":"doctoraccess1234",
        "password2":"doctoraccess1234"
    },
    "profile_data": {
        "address": "Dortmund",
        "mobile": "12312343424"
    }
}


POST api/doctor/login/

Details: API endpoint for doctor login. Admin needs to approve account otherwise login will not be successful.

request body:

{
    "username": "doctor1",
    "password": "doctoraccess1234"
}

POST api/v1/pet/registration/

Details: API endpoint for creating new patient account.

request:

{
    "user_data": {
        "username": "patient2",
        "first_name": "patien2",
        "last_name": "two",
        "password":"patientaccess1234",
        "password2":"patientaccess1234"
    },
    "profile_data": {
        "pet_age": "3",
        "pet_name": "Juli",
        "owner_address": "Dhaka",
        "owner_mobile": "12312343424"
    }
}


POST api/pet/login/

Details: API endpoint for patient login. Account needs be approved by admin first.

request:

{
    "username": "patient2",
    "password": "patientaccess1234"
}
