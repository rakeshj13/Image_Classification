
    <title>CIFAR-10 Image Classification using CNN and ANN</title>

    <h1>Overview</h1>
    <p>This project demonstrates the use of Convolutional Neural Networks (CNNs) to classify images from the CIFAR-10 dataset into 10 distinct categories: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck.</p>
    <p>The project compares the performance of a basic Artificial Neural Network (ANN) with a CNN model and highlights the superior accuracy of CNNs for image classification tasks.</p>

    <h2>Dataset</h2>
    <p>The CIFAR-10 dataset consists of 60,000 32x32 color images divided into 10 categories:</p>
    <ul>
        <li>Training Set: 50,000 images</li>
        <li>Test Set: 10,000 images</li>
        <li>Each image is labeled with one of the 10 classes</li>
    </ul>

    <h2>Project Workflow</h2>
    
    <h3>Data Loading and Preprocessing</h3>
    <p>The dataset is loaded using TensorFlow's <code>datasets.cifar10</code> module.</p>
    <p>Images are normalized by scaling pixel values to the range [0, 1].</p>
    
    <h3>ANN Model</h3>
    <p>A basic Artificial Neural Network with dense layers is implemented.</p>
    <p>Achieved ~49% accuracy on the test set.</p>
    
    <h3>CNN Model</h3>
    <p>A Convolutional Neural Network is implemented with the following architecture:</p>
    <ul>
        <li>2 Convolutional Layers with MaxPooling</li>
        <li>Flatten layer</li>
        <li>Fully connected Dense layers with ReLU and Softmax activation functions</li>
    </ul>
    <p>Achieved ~70% accuracy on the test set, outperforming the ANN.</p>
    
    <h3>Evaluation</h3>
    <p>Models are evaluated using metrics like accuracy, precision, recall, and F1-score.</p>
    <p>Confusion matrices and classification reports provide detailed performance insights.</p>

    <h2>Results</h2>
    <div class="table-container">
        <table>
            <thead>
                <tr>
                    <th>Model Type</th>
                    <th>Test Accuracy</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>ANN</td>
                    <td>~49%</td>
                </tr>
                <tr>
                    <td>CNN</td>
                    <td>~70%</td>
                </tr>
            </tbody>
        </table>
    </div>
