Set ubuntu layout to portuguese

setxkbmap -model abnt2 -layout br

create virtual env
python3 -m venv .env

Activate virtual environment
source .env/bin/activate

Install libraries into virtual environment
pip install -r requirements.txt

Deactivate virtual environment
deactivate

First clone
sudo git clone - repos name

# To DO
- Add a library to create branch with good practices. Ec: FEATURE_xxx_XXX