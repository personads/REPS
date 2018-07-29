Relative Entropy Policy Search
===

[REPS by Peters et al., 2010][1] is an approach to tackle the optimisation bias and information loss often associated with continuous control Reinforcement Learning tasks by introducing an upper bound by which both the policy and value functions are allowed to change. Extending the approach by [van Hoof et al., 2017][2], this research project by Knegt, Kuric, Müller-Eberstein and Scheffers aims to extend REPS to deep neural network models which perform tasks within [OpenAI Gym][3].


Requirements
---
This project is written in Python3 and requires the dependencies listed in the `requirements.txt` file. These include:

* [numpy][4]
* [scipy][5]
* [matplotlib][6]
* [PyTorch][7]
* [OpenAI Gym][3] with [MuJoCo][8]

Please follow each respective installation guide if necessary.


Running Gym Tasks
---
Scripts to run gym tasks for `Pendulum-v0`, `Swimmer-v2`, `HalfCheetah-v2` as well as `Reacher-v2`, `Hopper-v2` you can use the apprpriate scripts in the `run/` directory.

```
$ python3 run/pendulum.py
```

The models of each iteration are saved as `.pth` files and the evaluation results should be rendered every two iterations.


Results
---
Rendered results of the best performing model configurations for `Pendulum-v0`, `Swimmer-v2` and `HalfCheetah-v2` can be found on YouTube:

* [`Pendulum-v0`](https://www.youtube.com/watch?v=qzp4KwlxYFQ)
* [`Swimmer-v2`](https://www.youtube.com/watch?v=L4pFPi5X8Ok)
* [`HalfCheetah-v2`](https://www.youtube.com/watch?v=uTC0B1ms_iA)

Further plots and result numbers can be found within the `results/` directory.

References
---
[1]: https://www.aaai.org/ocs/index.php/AAAI/AAAI10/paper/viewFile/1851/2264  
*Peters, J., Mulling, K., and Altün, Y. Relative entropy policy search. In Fox, M. and Poole, D. (eds.), Proceedings of the Twenty-Fourth AAAI Conference on Artificial Intelligence (AAAI 2010), pp. 1607–1612. AAAI Press, 2010.*

[2]: http://jmlr.org/papers/v18/16-142.html  
*van Hoof, H., Neumann, G., and Peters, J. Non-parametric policy search with limited information loss. Journal of Machine Learning Research, 18(73):1–46, 2017.*

[3]: https://arxiv.org/abs/1606.01540  
*Brockman, G., Cheung, V., Pettersson, L., Schneider, J., Schulman, J., Tang, J., and Zaremba, W. Openai G      ym. CoRR, abs/1606.01540, 2016.*

[4]: http://www.numpy.org/
[5]: https://scipy.org/
[6]: https://matplotlib.org/
[7]: https://pytorch.org/
[8]: http://mujoco.org/