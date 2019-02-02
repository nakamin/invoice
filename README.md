# What is this?
This is a script that I put together to automagically
generate invoices for my contract work. The tool will
produce invoices with a date, invoice number, and line
items with rate, quantity. The line item prices are summed
and displayed as a total for the clients convenience.

# How do I use this?
## Customization
You should first change the constants in the script to the
values that apply for you. They are all at the top of the file
so it's easy to find them. Also if you are not currently at invoice
number 0 then you will need to change the `num.txt` file.

## Running
This is a commandline tool. You run it just like any other
python script, but you will need some packages installed.
The dependencies are: `docx-mailmerge` and `comtypes`. The first
is used to insert the inputted quantities into the word document,
and the second is used to convert the Word document to a PDF.
I would suggest that you setup a virtual env so that installing
the packages is less of a pain. I also have a batch script that I
double click to run the script, I've included it in the repo.

# What if I don't like the way the template looks?
You can edit the template to fit your needs, but don't change anything
in angle brackets, those are mail merge feilds used by the script to
inject the data you input. If all you need is a simple invoice in the
format that I have here then you shouldn't have any issues. If you need
additional features, you should probably read the code and add them yourself.
I tried to document it so that it's easy to understand.
