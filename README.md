# temp_converter
def temperature_converter(temperature, input_unit, output_unit):
    if input_unit == 'C' and output_unit == 'F':
        return temperature * 9 / 5 + 32
    elif input_unit == 'F' and output_unit == 'C':
        return (temperature - 32) * 5 / 9
    else:
        return temperature

temp = float(input('Enter temperature: '))
input_unit = input('Enter input unit (C or F): ')
output_unit = input('Enter output unit (C or F): ')
converted_temp = temperature_converter(temp, input_unit, output_unit)
print(f'{temp} {input_unit} is equal to {converted_temp} {output_unit}')
