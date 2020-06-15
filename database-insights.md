# Insights of contruct Database

## Some Tips

- All of data collect is to show for a unic vehicle
- Database is to be able to add many vehicles of many users

# Index

1. DataCar to collect
2. DataUsers to collect
3. Database Example

# DataCar to collect

- CarStatus

  - Locked<Boolean>: true || false
  - Battery<Number>: 54
  - AvailableRange<Number>: 297(km/h)
  - TotalDistance<Number>: 36012.12(km)
  - Weight<Number>: 1200(Kilograma)
  - TemperatureInside<Number>: 27(Célsius)
  - TemperatureOutside<Number>: 34(Célsius)
  - Humitity<Number>: 46(%)
  - Pressure<Number>: 998(hPa)
  - Wind<Number>: 5.6(km/h)

- A/C

  - Status<Boolean>: true || false
  - TemperatureSetted<Number>: 25 (Célsius)
  - FanSpeed<number>: range(1-5)
  - Mode<String>: "auto" || "dry" || "coll" || "program"

- Controls

  - Lights<Boolean>: true || false => RETIRAR
  - FrontTrunk<Boolean>: true || false
  - Trunk<Boolean>: true || false
  - FrontLeftDoor<Boolean>: true || false
  - FronRightDoor<Boolean>: true || false
  - BackLeftDoor<Boolean>: true || false
  - BackRightDoor<Boolean>: true || false
  - ChargePort<Boolean>: true || false

- System

  - OwnerId<String>: "4e10aa9a-a696-4881-8154-0ae9d86b7a45"(uuid)
  - Time<Date>: 13 Jun 2020 18:39:00 GMT
  - ModelYear<Number>: 2018
  - CarReview<Date>: 23 May 2020 09:00:00 GMT
  - Insurance<Date>: 02 Oct 2022 09:00:00 GMT

- Model
  - Description<String>
  - Chassi<String>: "7176267SJWUB821JJHS"
  - Engine<Number>: 188(hp)
  - DriveType<String>: 4WD
  - Transmission<String>: "Automatic" || "Manual"
  - Fuel<String>: "Diesel"
  - TopSpeed<Number>: 230(km/h)
  - ZeroToHundred<Number>: 7(s)

OPCIONAIS

- CarStatus

  - Energy<Number>: 45(%) => Eletric car
  - FuelReservatory<Number>: 70(%) => Fuel car
  - BreakFluid<Number>: 9(%)
  - TireWear<Number>: 25(%)

- Location
  - Latitude<Number>: 72373734737
  - Longitude<Number>: 72625635347
  - Accuracy<Number>: 5(m)
  - Speed<Number>: 12(m/s)
  - Altitude<Number>: 200(m)
  - AltitudeAccuracy<Number>: 20(m)

# DataUsers to collect

- User

  - OwnerId<String>: "4e10aa9a-a696-4881-8154-0ae9d86b7a45"(uuid)
  - Name<String>: "Leandro"
  - Surname<String>: "Chaves"
  - Email: "leadrofchaves@outlook.com"
  - Password: "123456"
  - Address:: Rua Gurgel 11"
  - createdAt<Date>: Date
  - updatedAt<Date>: Date
  - deletedAt<Date>: Date || null

- Vehicle[]
  - Id<String>: "4e10aa9a-a696-4881-8154-0ae9d86b7a45"(uuid)
  - DataCar<DataCar>: {DataCar}

# Database Example

- Verify `db.json`
