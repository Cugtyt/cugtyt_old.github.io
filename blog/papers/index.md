# **Blogs of Papers**

## Contact me

* Blog -> <https://cugtyt.github.io/blog/index>
* Email -> <cugtyt@qq.com>, <cugtyt@gmail.com>
* GitHub -> [Cugtyt@GitHub](https://github.com/Cugtyt)

---

本系列博客主要是关于阅读论文的笔记。

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