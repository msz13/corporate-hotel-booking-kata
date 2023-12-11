Hotel Kata

Booking
  * Booking should contain a unique ID, employeeId, hotelId, roomType, checkIn and checkOut.
Scenario: Employ see booking confirmation
  *	Check out date must be at least one day after the check in date.
Scenario: Chceckout validation
  *	Validate if the hotel exists and room type is provided by the hotel
Scenario: Failure hotel doesn’t exists
Scenario: Failure room type doesn’t exists in hotel
  *	Booking should only be allowed if there is at least one room type available during the whole booking period.
Scenario: Failure where no room is avaible
Scenario: Failure where room type is not evaible, but another is avaiple
  *	Verify if booking is allowed according to the booking policies defined, if any. See Booking Policy Service for more details.
Scenario: Failue booking is not allowed based on polices TO SPECIFY
  *	Keep track of all bookings. E.g. If hotel has 5 standard rooms, we should have no more than 5 bookings in the same day.
Scenario: Many booking for same room type in one day when they are avaible
Scenario: Many booking for same room type in one day when they are not avaible
  *	Hotel rooms can be booked many times as long as there are no conflicts with the dates.
Scenario: Bookings for different days
Scenario set: Failure bookings when dates are overlapping
