# nbdev2
Creating a nbdev2 work environment and a library with it
**********************************
## References
1. Youtube: [nbdev tutorial -- zero to published project in 90 minutes](https://youtu.be/l7zS8Ld4_iA)
2. Tutorial: [nbdev tutorial](https://nbdev.fast.ai/tutorial.html)
3. Repo: [fastai / nbdev](https://github.com/fastai/nbdev)
## Steps
1. To setup the environment:
WSL
```
$ mamba create -n nbdev2 python=3.9
$ mamba activate nbdev2
(nbdev2) $ mamba install -c anaconda notebook
(nbdev2) $ mamba install -c fastai nbdev
```
2. Clone a basic github repo:
```
(nbdev2) $ git clone git@github.com:fmussari/nbdev2_cards.git
(nbdev2) $ cd nbdev2_cards
```
3. Program Card Class in [00_cards.ipynb](00_cards.ipynb)
4. Create [card.py](nbdev2_cards/card.py)
```
(nbdev2) $ nbdev_export
(nbdev2) $ pip install -e .
```
5. Since the path has underscore, and the library cannot. Change underscore with dash in lib_name [settings.ini](settings.ini) and change also the path:
```
lib_name = nbdev2-cards
lib_path = nbdev2_cards

```