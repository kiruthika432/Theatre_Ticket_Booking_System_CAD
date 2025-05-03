# Theatre_Ticket_Booking_System_CAD
.
        Project: Theatre Ticket Booking System
          Title: ShowSaga
Target Audience: Theatre owners / admins
           Type: B2B
      End Users: Families, Friends group, Tourists, Theatre enthusiasts
       Timeline: 2 to 3 weeks
      Team Size: 1 member
      
Features and Workflow:
                 1, Registration Page
                 2, Login Page
                 3, Add Movie details( movie name, genre, description, actor & actress name)
                 4, Add number of shows
                 5, Fix show timings
                 6, Select screen / hall
                 7, Customize seat layout
                 8, Set pricing by category
                 9, Enable seat blocking
                 10, Set timelimit for booking and cancellation
                 11, Auto revenue calculation 
                 12, Get ratings and feedback from users
                 13, Display ratings

System Design:
        1, Class RegistrationPage:
                -       TheatreID: int
                -     TheatreName: String
                -        location: String
                -        userName: String
                -        password: String
                - confirmPassword: String
.
        2, Class LoginPage:
                - userName: String
                - password: String
.
        3, Class Movie:
                -          ID: int
                -       title: String
                -       genre: String
                - description: String
                -   actorName: String
                - actressName: String
.
        4, Class Show:
                -       movie: Movie ( class 3)
                -    showTime: String
                -        hall: Hall
.
        5, Class Hall:
                -   hallName: String
                - seatLayout: SeatLayout (class 6)
.
        6, Class SeatLayout:
                -    rows: int
                - columns: int
                -   seats: List<Seat>
.
        7, Class PricingRule
                - category: String
                -    price: double
.
        8, Class Booking
                -        show: Show ( class 4)
                - bookedSeats: List<Seat>
                -    bookedAt: String
                - cancelledAt: String
.
        9, Class RatingandFeedback:
                -   movie: Movie (class 3)
                -  rating: int
                - comment: String
.
        10, Class RevenueTracker:
                -         show: Show ( class 4)
                - totalRevenue: double





![Screenshot from 2025-05-03 15-10-24](https://github.com/user-attachments/assets/d72f44f3-3198-4cd3-b1c8-02c2e1d28aa4)







      

