# TF2-Item-list
I could not find a JSON version of the tf2 item scema, so I made my own.
FYI: This only contains the item defindexes. This is trimmed down from the original.
Here is the python code I used:
import json
import vdf

if __name__ == '__main__':

    item_table_file = open(your tf2 file name)
    item_table = vdf.parse(item_table_file)["items"]

    file = open(output, 'x')

    json.dump(item_table, file)
