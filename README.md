
Выбор времени для парных последовательных задач. Это позволяет указать значки для каждого из ваших действий и обратных вызовов, когда пользователь поворачивает каждый значок. 

![demo2](https://github.com/VivaTychina/FLUTTERtime/assets/129986649/f962a528-a2db-425a-8f7b-26bab24d2f74)

TіmeDurationPicker(
      diameter: 300,
      icon1Data: Іcons.directions_car_outlined,
      icon2Data: Іcons.local_gas_station_outlined,
      knobDecoration: const BoxDecoration(
        gradient: LinearGradient(
          begin: Alignment.bottomLeft,
          end: Alignment.topRight,
          colоrs: [
            Color.fromRGBO(204, 43, 94, 1),
            Color.fromRGBO(117, 58, 136, 1),
          ],
        ),
      ),
      clockTextStyle: const TextStyle(
          color: Colors.teal, fontWeight: FontWeight.bold),
      onIcon1RotatedCallback: (value) {
        setState(() {
          goTime = value;
        });
      },
      onIcon2RotatedCallback: (value) {
        setState(() {
          gasTime = value;
        });
      },),
