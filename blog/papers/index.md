# **Blogs of Papers**

## Contact me

* Blog -> <https://cugtyt.github.io/blog/index>
* Email -> <cugtyt@qq.com>, <cugtyt@gmail.com>
* GitHub -> [Cugtyt@GitHub](https://github.com/Cugtyt)

---

本系列博客主要是关于阅读论文的笔记。

---

## [**Evaluation of a Tree-based Pipeline Optimization Tool for Automating Data Science**](https://cugtyt.github.io/blog/papers/2019/0728)

> TPOT，通过遗传算法自动化的探索管道，包括预处理，模型选择，参数设置等。

---

## [**MIXED PRECISION TRAINING**](https://cugtyt.github.io/blog/papers/2019/0714)

> 混合精度训练，一些方法可以让FP16的运算达到FP32的效果，但是内存减少，速度提升。

---

## [**TRAINING CONFIDENCE-CALIBRATED CLASSIFIERS FOR DETECTING OUT-OF-DISTRIBUTION SAMPLES**](https://cugtyt.github.io/blog/papers/2019/0724)

> 检测内分布和外分布，通过GAN生成靠近内分布的外分布，让分类器通过KL散度使得外分布的预测为均匀分布，可以让分类器更加鲁棒。

---

## [**Deep Video Inpainting**](https://cugtyt.github.io/blog/papers/2019/0712)

> 基于图像编码器-解码器的模型，收集提炼邻近帧的信息，然后生成未知的区域。同时，输出通过循环反馈和时间记忆模块保持时间上的一致性。效果好，速度近乎实时。

---

## [**Fast Online Object Tracking and Segmentation: A Unifying Approach**](https://cugtyt.github.io/blog/papers/2019/0710)

> 用单个方法实时做到同时目标跟踪和半监督视频目标分割。SiamMask通过二值分割任务增强损失提升了全卷积Siamense目标跟踪方法的训练过程。训练完成后，SiamMask只依赖于单个边界框初始值，可以做到旋转的边界框分割未知类别目标，达到每秒55帧。

---

## [**“IMAGENET-TRAINED CNNS ARE BIASED TOWARDS TEXTURE; INCREASING SHAPE BIAS IMPROVES ACCURACY AND ROBUSTNESS**](https://cugtyt.github.io/blog/papers/2019/0708)

> 证明了传统的模型使用纹理来识别，创建数据集Stylized-ImageNet（风格迁移，保留形状，换掉纹理），可以作为数据扩充，而且学到形状特征比原来的性能更高

---

## [**“Why Should I Trust You?” Explaining the Predictions of Any Classifier**](https://cugtyt.github.io/blog/papers/2019/0614)

> LIME 解释模型

---

## [**SNIP: SINGLE-SHOT NETWORK PRUNING BASED ON CONNECTION SENSITIVITY**](https://cugtyt.github.io/blog/papers/2019/0612)

> 分析连接重要性进行剪枝，Single-Shot

---

## [**THE LOTTERY TICKET HYPOTHESIS: FINDING SPARSE, TRAINABLE NEURAL NETWORKS**](https://cugtyt.github.io/blog/papers/2019/0611)

> 文章关于神经网络剪枝。做法是四步：
> 
> 初始化，训练一段时间，对梯度小的p%设置mask不再更新，将原始的初始化权重赋值回现在没有剪枝的部分
>
> 彩票假说，即原始网络中存在一些一开始就中奖的子网络，通过训练把中奖的找出来（这里只找一个），然后这个找到的子网络的初始权重是中奖的重要因素，需要再次赋值回来，如果重新对这个中奖子网络初始化，就无法拥有好的性能，证明了初始化的重要性。

---


## [**A New Backpropagation Algorithm withoutGradient Descent**](https://cugtyt.github.io/blog/papers/2019/0605)

> 用Moore-Penrose伪逆做反向传播，没看出来这篇文章有什么意义

---

## [**AutoAugment: Learning Augmentation Strategies from Data**](https://cugtyt.github.io/blog/papers/2019/0603)

> 使用强化学习策略搜索数据增强方法，奖励是验证集准确率

---

## [**DATASET DISTILLATION**](https://cugtyt.github.io/blog/papers/2019/0529)

> 将数据集压缩到少量合成数据中，可以少量训练达到很高的准确率。文章还展示了恶意数据攻击，以及预训练模型在新数据上的情况。

---

## [**Co-teaching: Robust Training of Deep Neural Networks with Extremely Noisy Labels**](https://cugtyt.github.io/blog/papers/2019/0510)

> 网络具有记忆特性，即网络最开始先学习容易学的，也可以看作是学到不带噪声数据更容易，然后才过拟合。co-teaching使用初始化不同两个网络交替学习，即学习到损失小的样本作为知识传到另一个网络中，这样两个网络的结构可以互相消除噪声的影响。

---

## [**DARTS: DIFFERENTIABLE ARCHITECTURE SEARCH**](https://cugtyt.github.io/blog/papers/2019/0509)

> 将离散的网络结构搜索转为连续优化问题，使用梯度下降求解。先搜索到最好的基本块，然后使用基本块搭建模型。相比于其他方法GPU用时有几个数量级的缩减。

---

## [**Connecting Generative Adversarial Networks and Actor-Critic Methods**](https://cugtyt.github.io/blog/papers/2019/0418)

> GAN和Actor-Critic之间的联系和二者目前研究方法的共通性。

---

## [**SeqGAN: Sequence Generative Adversarial Nets with Policy Gradient**](https://cugtyt.github.io/blog/papers/2019/0403)

> 使用强化学习中的梯度策略来让GAN生成离散序列数据。

---

## [**失之交臂的灵感-卷积权重标准化**](https://cugtyt.github.io/blog/papers/2019/0402)

> 曾经有过把权重初始化作为一种帮助网络训练的方法,但是当时没有做出来,现在看到了有篇文章把这个想法做出来了,灵感失之交臂。

---

## [**ACTIVATION MAXIMIZATION GENERATIVE ADVERSARIAL NETS**](https://cugtyt.github.io/blog/papers/2019/0219)

> AM GAN，AM Score作为生成样本质量指标，IS作为多样性指标，分析了类别信息对于生成样本的关系。

---

## [**UNSUPERVISED AND SEMI-SUPERVISED LEARNING WITH CATEGORICAL GENERATIVE ADVERSARIAL NETWORKS**](https://cugtyt.github.io/blog/papers/2019/0218)

> CatGAN，一个无监督和半监督学习的框架，将神经网络分类器与对抗生成模型相结合，该模型将经过判别训练的分类器正规化，也能够生成高质量的图像。

---

## [**PAYING MORE ATTENTION TO ATTENTION: IMPROVING THE PERFORMANCE OF CONVOLUTIONAL NEURAL NETWORKS VIA ATTENTION TRANSFER**](https://cugtyt.github.io/blog/papers/2019/0114)

> 注意力迁移和蒸馏

---

## [**Statistical Modeling: The Two Cultures**](https://cugtyt.github.io/blog/papers/2019/0113)

> 统计建模的两种文化

---

## [**Demystifying Parallel and Distributed Deep Learning: An In-Depth Concurrency Analysis**](https://cugtyt.github.io/blog/papers/2018/1123)

> 对于并行和分布式深度学习的综述。主要的算法，结构，形式，分析比较的方法。

---

## [**tempoGAN: A Temporally Coherent, Volumetric GAN for Super-resolution Fluid Flow**](https://cugtyt.github.io/blog/papers/2018/1119)

> 在四维空间使用GAN生成动态的烟雾，使用了两个判别器，一个是空间上的，一个是时间上的，用于控制生成的烟雾具有短暂的相关性，以模拟真实的情况。能够生成高分辨率的细节，使用了物理感知的数据增强，在2维和3维上证明了可行性。但是训练时间特别长，微调也是很耗时的过程。

---

## [**Grad-CAM++: Generalized Gradient-based Visual Explanations for Deep Convolutional Networks**](https://cugtyt.github.io/blog/papers/2018/0913)

> 一个新的可视化方法，源于Grad-CAM但是效果更好，并提供了数学推导，对像素位置的加权，解决了Grad-CAM无法定位同一图像中多个同类目标，以及对目标识别不完全的缺点，而且做了知识蒸馏，效果表现很好。

---

## [**Cyclical Learning Rates for Training Neural Networks**](https://cugtyt.github.io/blog/papers/2018/1005)

> 使用循环学习率的方法可以更提升训练效果

---

## [**Improved Techniques for Training GANs**](https://cugtyt.github.io/blog/papers/2018/0909)

> 提出了IS分数来衡量生成图像的质量，和人类判断很相关。提出了一些提升GAN的方法，Feature matching设定新的目标函数，解决GAN的不稳定性。Minibatch discrimination通过多个样本来解决模式坍塌的情况。Historical averaging在每层损失函数中加入一项，可以在低维、连续非凸博弈中找到平衡。Virtual batch normalization解决批标准化导致网络对于一个输入样本x的输出高度依赖于在这个批量中其他的几个输入x'。

---

## [**Critiquing an Article**](https://cugtyt.github.io/blog/papers/2018/0907)

> 如何写文章评论

---

## [**How good is my GAN?**](https://cugtyt.github.io/blog/papers/2018/0830)

> 提出了GAN生成图像的衡量标准。GAN-train和GAN-test，类似于准确率和召回率，分别为用生成图像训练，真实图像测试，和真实图像训练，生成图像测试。对现有的一些模型进行了对比，发现该衡量方法可以对生成图像质量和图像多样性定量衡量，比IS和FID更有效。

---

## [**One pixel attack for fooling deep neural networks**](https://cugtyt.github.io/blog/papers/2018/0827)

> 通过只修改自然图像的一个像素可以让网络错判，实验使用了全卷积网络，VGG，NiN，修改1，3，5个像素点，分为有目标攻击和无目标攻击，分别为将真实类别攻击为目标类别或将真实类别攻击为其他类别，结果证明修改1个像素已经能让很多网络很多类别错判，增加像素点可以增大成功率。

---

## [**LightGBM: A Highly Efficient Gradient Boosting Decision Tree**](https://cugtyt.github.io/blog/papers/2018/0823)

> 提出了新的GBDT算法，包括了两个新方法：基于梯度的单边采样和互斥特征打包，两个方法分别用于处理数据实例较多和特征较多的情况。GOSS排除了大部分梯度小的数据，用梯度大的数据来计算信息增益，在数据量较小的时候也能获得精确度很高的增益估计。EFB对互斥的特征进行打包，减少特征数量，使用贪心的算法可以达到很好的近似率。这个方法提高了速度，超越了现有的方法。

---

## [**XGBoost: A Scalable Tree Boosting System**](https://cugtyt.github.io/blog/papers/2018/0820)

> 提出了一个Tree Boosting系统，高效可扩展。提出了针对于稀疏数据的稀疏感知算法，方法是为树节点加入默认的方向，以做到更好的数据分割，数据压缩，缓存访问模式和数据共享是系统的关键因素。数据压缩是使用块的结构，对列进行压缩，缓存访问使用不同进程对块进行读写处理，数据通过硬盘之间轮换共享。

---

## [**Squeeze-and-Excitation Networks**](https://cugtyt.github.io/blog/papers/2018/0818)

> 压缩激活，自适应校准，SE块的结构可以用于很多网络，提升性能

---

## [**Aggregated Residual Transformations for Deep Neural Networks**](https://cugtyt.github.io/blog/papers/2018/0817)

> 复杂度一致的情况下，增加基数比宽度和深度更有效，使用重复相同拓扑结构的方法简化模型设计

---

## [**ShuffleNet V2: Practical Guidelines for Efficient CNN Architecture Design**](https://cugtyt.github.io/blog/papers/2018/0814)

> 使用速度而不是FLOPs来衡量模型的效率，提出设计高效网络的几条原则，并根据原则设计了ShuffleNet V2

---

## [**Xception: Deep Learning with Depthwise Separable Convolutions**](https://cugtyt.github.io/blog/papers/2018/0813)

> 关于Inception的假说，把Inception模块替换为深度可分卷积，参数数量和V3差不多，性能更好

---

## [**ShuffleNet: An Extremely Efficient Convolutional Neural Network for Mobile**](https://cugtyt.github.io/blog/papers/2018/0812)

> 点级别的组卷积和通道重排导致复杂度减少，比MobileNet更好

---

## [**[Cycle GAN] Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks**](https://cugtyt.github.io/blog/papers/2018/0811)

> 在无数据对的情况下学习转换，学习x->y->x，损失有对抗损失和环形一致损失

---

## [**[CoordConv] An intriguing failing of convolutional neural networks and the CoordConv solution**](https://cugtyt.github.io/blog/papers/2018/0809)

> 相比普通卷积加入了坐标层，在一些问题上比普通卷积好很多

---

## [**Mask R-CNN**](https://cugtyt.github.io/blog/papers/2018/0808)

> 相比Faster R-CNN加入了一个掩模分支用于生成掩模，在其他任务上表现不错

---

## [**Faster R-CNN**](https://cugtyt.github.io/blog/papers/2018/0807)

> 对区域提议使用网络生成，这个网络和目标检测网络共享特征，速度更快，效果更好

---

## [**Fast R-CNN**](https://cugtyt.github.io/blog/papers/2018/0805)

> R-CNN and SPPnet缺陷，一步到位的训练，使用多任务损失，RoI pooling layer，Truncated SVD

---

## [**[R-CNN] Rich feature hierarchies for accurate object detection and semantic segmentation**](https://cugtyt.github.io/blog/papers/2018/0803)

> 自底向上区域提议+CNN

---

## [**YOLOv3: An Incremental Improvement**](https://cugtyt.github.io/blog/papers/2018/0802)

> 对网络结构做了一些变动

---

## [**YOLO9000: Better, Faster, Stronger**](https://cugtyt.github.io/blog/papers/2018/0731)

> 使用一些方法提升了YOLO的性能，使用聚类设置框维度，使用分类数据和检测数据联合训练

---

## [**You Only Look Once: Unified, Real-Time Object Detection**](https://cugtyt.github.io/blog/papers/2018/0728)

> YOLO只使用一个神经网络，用回归问题解决目标检测，速度快，相比R-CNN准确率还差点

---

## [**Wasserstein GAN**](https://cugtyt.github.io/blog/papers/2018/0727)

> EM与其他距离和散度的比较，WGAN可以提升稳定性，更好的收敛

---

## [**Are GANs Created Equal? A Large-Scale Study**](https://cugtyt.github.io/blog/papers/2018/0725)

> fair and comprehensive comparison of the state-of-the-art GANs, it is necessary to report a summary of distribution of results, a series of tasks of increasing difficulty for which undisputed measures.  
> We find that most models can reach similar scores with enough hyperparameter optimization and random restarts. This suggests that improvements can arise from a higher computational budget and tuning more than fundamental algorithmic changes.

---

## [**The GAN Landscape: Losses, Architectures, Regularization, and Normalization**](https://cugtyt.github.io/blog/papers/2018/0723)

> losses, regularization and normalization schemes, and neural architectures, and their impact on the on the quality of generated samples which we assess by recently introduced quantitative metrics.

---

## [**MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications**](https://cugtyt.github.io/blog/papers/2018/0721)

> Depthwise Separable Convolution, Width Multiplier: Thinner Models, Resolution Multiplier: Reduced Representation

---