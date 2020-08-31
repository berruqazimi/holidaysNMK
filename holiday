import datetime
import sys
import json
import argparse
parser = argparse.ArgumentParser()
parser.add_argument('--day', help='Day , REQUIRED', required=True)
args, unknown = parser.parse_known_args()
try:
    def is_holiday (day):
        New_Year = datetime.date(2020,1,1)
        Orthodox_Christmas_Day = datetime.date(2020, 1, 7)
        Orthodox_Easter_Monday =  datetime.date(2020, 4, 20)
        Labour_Day = datetime.date(2020, 5, 1)
        Eid_Al_Fitr = datetime.date(2020, 5, 23)
        Saints_Cyril_and_Methodius_Day = datetime.date(2020, 5, 24)
        Republic_Day = datetime.date(2020, 8, 2)
        Independence_Day = datetime.date(2020, 9, 8)
        People_Uprising_Against_Fascism_Day = datetime.date(2020, 10, 11)
        Day_of_the_Macedonian_Revolutionary_Struggle = datetime.date(2020, 10, 23)
        Kliment_Ohridski_Day = datetime.date(2020, 12, 8)
        if day == New_Year:
            return 'New Year'
        if day == Orthodox_Christmas_Day:
            return 'Orthodox Christmas Day'
        if day == Orthodox_Easter_Monday:
            return 'Orthodox Easter Monday'
        if day == Labour_Day:
            return 'Labour Day'
        if day == Eid_Al_Fitr:
            return 'Eid Al-Fitr'
        if day == Saints_Cyril_and_Methodius_Day:
            return 'Saints Cyril and Methodius Day'
        if day == Republic_Day:
            return 'Republic Day'
        if day == Independence_Day:
            return 'Independence Day'
        if day == People_Uprising_Against_Fascism_Day:
            return "People's Uprising Against Fascism_Day"
        if day == Day_of_the_Macedonian_Revolutionary_Struggle:
            return "Day of the Macedonian Revolutionary Struggle"
        if day == Kliment_Ohridski_Day:
            return "Kliment Ohridski's Day"
        else:
            return "Is not Holiday"
    holiday = is_holiday(args.day)
    result ={'Holiday': holiday}
    print(json.dumps(result))
    exit(0)
except Exception as e:
    sys.stderr.write(str(e))
    exit(-1)
