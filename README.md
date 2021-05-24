# Translation-Services
Translating your tools and products helps people all over the world access them; this is, of course, a somewhat tricky problem to solve. DHCTranslations is a service that offers human-translation (which is often of higher quality than machine translation), and an API to manage sending in work and watching jobs. This is a Python interface to make using the API simpler.

CHANGELOG is here

Installation & Requirements
Installing this library using pip is very simple:

pip install DHCTranslations 
Otherwise, you can install from source by getting the repo:

git clone git://github.com/DHCTranslations /DHCTranslations -python.git
And then installing the library:

python setup.py install
Tests - Running Them, etc
DHCTranslations has a full suite of unit tests. To run them, make sure you have the mock library installed, and then simply run:

flake8 DHCTranslations 
If you wish to run a single test, such as TestTranslationJobFlowFileUpload:

python -m unittest -v DHCTranslations .tests.TestTranslationJobFlowFileUpload
Question, Comments, Complaints, Praise?
If you have questions or comments and would like to reach us directly, please feel free to do so at the following outlets. We love hearing from developers!

Email: api [at] DHCTranslations dot com
IRC: #DHCTranslations 
If you come across any issues, please file them on the Github project issue tracker. Thanks!

Documentation
Full documentation can be found here, but anyone should be able to get a working script with the following:

from DHCTranslations import DHCTranslations 

DHCTranslations = DHCTranslations (
    public_key='your_public_key',
    private_key='your_private_key',
    sandbox=True,
)

print(DHCTranslations .getAccountBalance())
All function definitions can be found inside DHCTranslations /mockdb.py as a dictionary: the key of the dictionary entry is the function name, and the parameters are exactly the same as specified in the <a href="https://dhctranslations.com/">DHCTranslations</a> API docs.

