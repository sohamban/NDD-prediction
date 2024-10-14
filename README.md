Attention-Deficit/Hyperactivity Disorder (ADHD) is a prevalent type of neurodevelopmental disorder (NDD) that affects attention regulation, impulse control, and hyperactivity. In this research, the ADHD dataset was acquired from the widely used ADHD-200 portal, which provides neuroimaging data in functional magnetic resonance imaging (fMRI) format. The fMRI data captures the brain's functional activity by measuring changes in blood flow, allowing the study of neural connectivity patterns associated with ADHD.

To process and analyze this complex fMRI data, a combination of Group Independent Component Analysis (grouped ICA) and Group Dictionary Learning (grouped DL) techniques was employed. These methods are crucial in reducing the dimensionality of the data and extracting meaningful features by identifying common patterns across the dataset, which consists of time-series data reflecting neural activity over time.

The combined time-series data generated from these methods was then used to calculate the brain's functional connectivity through Phase Locking Value (PLV). PLV is a widely recognized method in neuroscience that measures the synchronization between two brain regions over time, reflecting the strength of their functional connectivity. This resulted in the creation of a Brain Functional Connectivity (BFC) matrix, representing how different brain regions interact with one another during specific tasks or resting states.

The next step involved classifying this BFC matrix using a Graph Convolutional Neural Network (GCN). Since brain connectivity can naturally be modeled as a graph, where brain regions are considered as nodes and the functional connections as edges, GCNs are well-suited for this task. Graph-based GCNs excel at learning from non-Euclidean data, like brain connectivity graphs, by capturing both local and global structural information. By leveraging the power of GCNs, this approach can more effectively analyze the complex relationships between brain regions and provide a deeper understanding of ADHD's neurofunctional underpinnings.

Thus, by using graph-based neural networks like GCNs, this method offers a novel and advanced way to classify ADHD patients based on their brain connectivity patterns, potentially leading to more accurate diagnoses and deeper insights into the disorder.
