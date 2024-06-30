Code smells are those bad code structures that violate design principles and make software systems difficult to understand and maintain. Although many techniques have been proposed, most approaches only detect one kind of code smell and fail to identify multiple smells simultaneously. Furthermore, existing multi-label detection approaches, e.g. the classifier chain, suffer from propagation errors along the chain. To this end, this paper proposes MultiSmell, a novel approach to detect multiple code smells simultaneously based on a heterogeneous graph. Firstly, we select 28 real-world projects as a corpus to construct the dataset. Both textual and metric features are extracted from these projects to generate the samples labeled with multiple code smells by static analysis and detection rules. Secondly, MultiSmell constructs a heterogeneous graph in which features and labels are abstracted into different types of nodes by XLNet, BiLSTM, and CNN models. To generate more expressive node representations, we built a layer to fuse the feature and label nodes by borrowing the message-passing mechanism of graph attention networks. Finally, after several rounds of updating iterations, the label nodes are fed into the multi-layer perceptron to detect multi-label code smells.We evaluate MultiSmell by answering 7 research questions. The experimental results show that our approach exhibits superior exactMatchRatio and F1 scores when detecting multi-label code smells. Furthermore, it improves accuracy by 10.96% and F1 by 8.54% on average compared to the existing approach, demonstrating its effectiveness.
