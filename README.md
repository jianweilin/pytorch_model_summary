# PyTorch model summary
pytorch model summary, statistic parameters number, memory usage, MAdd and so on

use ResNet50 as an example

                               module name   input shape  output shape  parameters quantity  memory       MAdd run time percent
    0                         conv1.Conv2d     3 224 224    64 112 112                 9408  0.03MB  235225088            3.55%
    1                      bn1.BatchNorm2d    64 112 112    64 112 112                  128  0.03MB    3211264            0.67%
    2                            relu.ReLU    64 112 112    64 112 112                    0  0.03MB     802816            0.79%
    3                    maxpool.MaxPool2d    64 112 112    64  56  56                    0  0.01MB    1605632            4.02%
    4                layer1.0.conv1.Conv2d    64  56  56    64  56  56                 4096  0.01MB   25489408            0.41%
    5             layer1.0.bn1.BatchNorm2d    64  56  56    64  56  56                  128  0.01MB     802816            0.17%
    6                layer1.0.conv2.Conv2d    64  56  56    64  56  56                36864  0.01MB  231010304            2.80%
    7             layer1.0.bn2.BatchNorm2d    64  56  56    64  56  56                  128  0.01MB     802816            0.15%
    8                layer1.0.conv3.Conv2d    64  56  56   256  56  56                16384  0.05MB  101957632            1.22%
    9             layer1.0.bn3.BatchNorm2d   256  56  56   256  56  56                  512  0.05MB    3211264            0.70%
    10                  layer1.0.relu.ReLU   256  56  56   256  56  56                    0  0.05MB     802816            0.41%
    11        layer1.0.downsample.0.Conv2d    64  56  56   256  56  56                16384  0.05MB  101957632            1.22%
    12   layer1.0.downsample.1.BatchNorm2d   256  56  56   256  56  56                  512  0.05MB    3211264            0.67%
    13               layer1.1.conv1.Conv2d   256  56  56    64  56  56                16384  0.01MB  102559744            1.19%
    14            layer1.1.bn1.BatchNorm2d    64  56  56    64  56  56                  128  0.01MB     802816            0.18%
    15               layer1.1.conv2.Conv2d    64  56  56    64  56  56                36864  0.01MB  231010304            2.80%
    16            layer1.1.bn2.BatchNorm2d    64  56  56    64  56  56                  128  0.01MB     802816            0.20%
    17               layer1.1.conv3.Conv2d    64  56  56   256  56  56                16384  0.05MB  101957632            1.31%
    18            layer1.1.bn3.BatchNorm2d   256  56  56   256  56  56                  512  0.05MB    3211264            0.67%
    19                  layer1.1.relu.ReLU   256  56  56   256  56  56                    0  0.05MB     802816            0.52%
    20               layer1.2.conv1.Conv2d   256  56  56    64  56  56                16384  0.01MB  102559744            1.19%
    21            layer1.2.bn1.BatchNorm2d    64  56  56    64  56  56                  128  0.01MB     802816            0.17%
    22               layer1.2.conv2.Conv2d    64  56  56    64  56  56                36864  0.01MB  231010304            2.94%
    23            layer1.2.bn2.BatchNorm2d    64  56  56    64  56  56                  128  0.01MB     802816            0.17%
    24               layer1.2.conv3.Conv2d    64  56  56   256  56  56                16384  0.05MB  101957632            1.37%
    25            layer1.2.bn3.BatchNorm2d   256  56  56   256  56  56                  512  0.05MB    3211264            0.73%
    26                  layer1.2.relu.ReLU   256  56  56   256  56  56                    0  0.05MB     802816            0.55%
    27               layer2.0.conv1.Conv2d   256  56  56   128  56  56                32768  0.03MB  205119488            1.95%
    28            layer2.0.bn1.BatchNorm2d   128  56  56   128  56  56                  256  0.03MB    1605632            0.38%
    29               layer2.0.conv2.Conv2d   128  56  56   128  28  28               147456  0.01MB  231110656            2.56%
    30            layer2.0.bn2.BatchNorm2d   128  28  28   128  28  28                  256  0.01MB     401408            0.09%
    31               layer2.0.conv3.Conv2d   128  28  28   512  28  28                65536  0.05MB  102359040            0.79%
    32            layer2.0.bn3.BatchNorm2d   512  28  28   512  28  28                 1024  0.05MB    1605632            0.35%
    33                  layer2.0.relu.ReLU   512  28  28   512  28  28                    0  0.05MB     401408            0.23%
    34        layer2.0.downsample.0.Conv2d   256  56  56   512  28  28               131072  0.05MB  205119488            1.48%
    35   layer2.0.downsample.1.BatchNorm2d   512  28  28   512  28  28                 1024  0.05MB    1605632            0.38%
    36               layer2.1.conv1.Conv2d   512  28  28   128  28  28                65536  0.01MB  102660096            0.87%
    37            layer2.1.bn1.BatchNorm2d   128  28  28   128  28  28                  256  0.01MB     401408            0.06%
    38               layer2.1.conv2.Conv2d   128  28  28   128  28  28               147456  0.01MB  231110656            2.15%
    39            layer2.1.bn2.BatchNorm2d   128  28  28   128  28  28                  256  0.01MB     401408            0.15%
    40               layer2.1.conv3.Conv2d   128  28  28   512  28  28                65536  0.05MB  102359040            0.79%
    41            layer2.1.bn3.BatchNorm2d   512  28  28   512  28  28                 1024  0.05MB    1605632            0.35%
    42                  layer2.1.relu.ReLU   512  28  28   512  28  28                    0  0.05MB     401408            0.20%
    43               layer2.2.conv1.Conv2d   512  28  28   128  28  28                65536  0.01MB  102660096            0.84%
    44            layer2.2.bn1.BatchNorm2d   128  28  28   128  28  28                  256  0.01MB     401408            0.09%
    45               layer2.2.conv2.Conv2d   128  28  28   128  28  28               147456  0.01MB  231110656            2.10%
    46            layer2.2.bn2.BatchNorm2d   128  28  28   128  28  28                  256  0.01MB     401408            0.09%
    47               layer2.2.conv3.Conv2d   128  28  28   512  28  28                65536  0.05MB  102359040            0.76%
    48            layer2.2.bn3.BatchNorm2d   512  28  28   512  28  28                 1024  0.05MB    1605632            0.38%
    49                  layer2.2.relu.ReLU   512  28  28   512  28  28                    0  0.05MB     401408            0.20%
    50               layer2.3.conv1.Conv2d   512  28  28   128  28  28                65536  0.01MB  102660096            0.87%
    51            layer2.3.bn1.BatchNorm2d   128  28  28   128  28  28                  256  0.01MB     401408            0.06%
    52               layer2.3.conv2.Conv2d   128  28  28   128  28  28               147456  0.01MB  231110656            2.10%
    53            layer2.3.bn2.BatchNorm2d   128  28  28   128  28  28                  256  0.01MB     401408            0.09%
    54               layer2.3.conv3.Conv2d   128  28  28   512  28  28                65536  0.05MB  102359040            0.79%
    55            layer2.3.bn3.BatchNorm2d   512  28  28   512  28  28                 1024  0.05MB    1605632            0.35%
    56                  layer2.3.relu.ReLU   512  28  28   512  28  28                    0  0.05MB     401408            0.17%
    57               layer3.0.conv1.Conv2d   512  28  28   256  28  28               131072  0.03MB  205320192            1.40%
    58            layer3.0.bn1.BatchNorm2d   256  28  28   256  28  28                  512  0.03MB     802816            0.20%
    59               layer3.0.conv2.Conv2d   256  28  28   256  14  14               589824  0.01MB  231160832            1.92%
    60            layer3.0.bn2.BatchNorm2d   256  14  14   256  14  14                  512  0.01MB     200704            0.06%
    61               layer3.0.conv3.Conv2d   256  14  14  1024  14  14               262144  0.05MB  102559744            0.70%
    62            layer3.0.bn3.BatchNorm2d  1024  14  14  1024  14  14                 2048  0.05MB     802816            0.20%
    63                  layer3.0.relu.ReLU  1024  14  14  1024  14  14                    0  0.05MB     200704            0.12%
    64        layer3.0.downsample.0.Conv2d   512  28  28  1024  14  14               524288  0.05MB  205320192            1.31%
    65   layer3.0.downsample.1.BatchNorm2d  1024  14  14  1024  14  14                 2048  0.05MB     802816            0.20%
    66               layer3.1.conv1.Conv2d  1024  14  14   256  14  14               262144  0.01MB  102710272            0.73%
    67            layer3.1.bn1.BatchNorm2d   256  14  14   256  14  14                  512  0.01MB     200704            0.06%
    68               layer3.1.conv2.Conv2d   256  14  14   256  14  14               589824  0.01MB  231160832            1.86%
    69            layer3.1.bn2.BatchNorm2d   256  14  14   256  14  14                  512  0.01MB     200704            0.06%
    70               layer3.1.conv3.Conv2d   256  14  14  1024  14  14               262144  0.05MB  102559744            0.70%
    71            layer3.1.bn3.BatchNorm2d  1024  14  14  1024  14  14                 2048  0.05MB     802816            0.20%
    72                  layer3.1.relu.ReLU  1024  14  14  1024  14  14                    0  0.05MB     200704            0.12%
    73               layer3.2.conv1.Conv2d  1024  14  14   256  14  14               262144  0.01MB  102710272            0.84%
    74            layer3.2.bn1.BatchNorm2d   256  14  14   256  14  14                  512  0.01MB     200704            0.09%
    75               layer3.2.conv2.Conv2d   256  14  14   256  14  14               589824  0.01MB  231160832            1.89%
    76            layer3.2.bn2.BatchNorm2d   256  14  14   256  14  14                  512  0.01MB     200704            0.06%
    77               layer3.2.conv3.Conv2d   256  14  14  1024  14  14               262144  0.05MB  102559744            0.73%
    78            layer3.2.bn3.BatchNorm2d  1024  14  14  1024  14  14                 2048  0.05MB     802816            0.23%
    79                  layer3.2.relu.ReLU  1024  14  14  1024  14  14                    0  0.05MB     200704            0.09%
    80               layer3.3.conv1.Conv2d  1024  14  14   256  14  14               262144  0.01MB  102710272            0.73%
    81            layer3.3.bn1.BatchNorm2d   256  14  14   256  14  14                  512  0.01MB     200704            0.03%
    82               layer3.3.conv2.Conv2d   256  14  14   256  14  14               589824  0.01MB  231160832            4.69%
    83            layer3.3.bn2.BatchNorm2d   256  14  14   256  14  14                  512  0.01MB     200704            0.06%
    84               layer3.3.conv3.Conv2d   256  14  14  1024  14  14               262144  0.05MB  102559744            0.96%
    85            layer3.3.bn3.BatchNorm2d  1024  14  14  1024  14  14                 2048  0.05MB     802816            0.29%
    86                  layer3.3.relu.ReLU  1024  14  14  1024  14  14                    0  0.05MB     200704            0.12%
    87               layer3.4.conv1.Conv2d  1024  14  14   256  14  14               262144  0.01MB  102710272            1.05%
    88            layer3.4.bn1.BatchNorm2d   256  14  14   256  14  14                  512  0.01MB     200704            0.06%
    89               layer3.4.conv2.Conv2d   256  14  14   256  14  14               589824  0.01MB  231160832            2.15%
    90            layer3.4.bn2.BatchNorm2d   256  14  14   256  14  14                  512  0.01MB     200704            0.06%
    91               layer3.4.conv3.Conv2d   256  14  14  1024  14  14               262144  0.05MB  102559744            0.70%
    92            layer3.4.bn3.BatchNorm2d  1024  14  14  1024  14  14                 2048  0.05MB     802816            0.20%
    93                  layer3.4.relu.ReLU  1024  14  14  1024  14  14                    0  0.05MB     200704            0.09%
    94               layer3.5.conv1.Conv2d  1024  14  14   256  14  14               262144  0.01MB  102710272            0.76%
    95            layer3.5.bn1.BatchNorm2d   256  14  14   256  14  14                  512  0.01MB     200704            0.09%
    96               layer3.5.conv2.Conv2d   256  14  14   256  14  14               589824  0.01MB  231160832            2.10%
    97            layer3.5.bn2.BatchNorm2d   256  14  14   256  14  14                  512  0.01MB     200704            0.06%
    98               layer3.5.conv3.Conv2d   256  14  14  1024  14  14               262144  0.05MB  102559744            0.73%
    99            layer3.5.bn3.BatchNorm2d  1024  14  14  1024  14  14                 2048  0.05MB     802816            0.18%
    100                 layer3.5.relu.ReLU  1024  14  14  1024  14  14                    0  0.05MB     200704            0.09%
    101              layer4.0.conv1.Conv2d  1024  14  14   512  14  14               524288  0.03MB  205420544            1.43%
    102           layer4.0.bn1.BatchNorm2d   512  14  14   512  14  14                 1024  0.03MB     401408            0.09%
    103              layer4.0.conv2.Conv2d   512  14  14   512   7   7              2359296  0.01MB  231185920            2.70%
    104           layer4.0.bn2.BatchNorm2d   512   7   7   512   7   7                 1024  0.01MB     100352            0.03%
    105              layer4.0.conv3.Conv2d   512   7   7  2048   7   7              1048576  0.05MB  102660096            0.96%
    106           layer4.0.bn3.BatchNorm2d  2048   7   7  2048   7   7                 4096  0.05MB     401408            0.14%
    107                 layer4.0.relu.ReLU  2048   7   7  2048   7   7                    0  0.05MB     100352            0.09%
    108       layer4.0.downsample.0.Conv2d  1024  14  14  2048   7   7              2097152  0.05MB  205420544            2.10%
    109  layer4.0.downsample.1.BatchNorm2d  2048   7   7  2048   7   7                 4096  0.05MB     401408            0.15%
    110              layer4.1.conv1.Conv2d  2048   7   7   512   7   7              1048576  0.01MB  102735360            1.14%
    111           layer4.1.bn1.BatchNorm2d   512   7   7   512   7   7                 1024  0.01MB     100352            0.03%
    112              layer4.1.conv2.Conv2d   512   7   7   512   7   7              2359296  0.01MB  231185920            2.53%
    113           layer4.1.bn2.BatchNorm2d   512   7   7   512   7   7                 1024  0.01MB     100352            0.03%
    114              layer4.1.conv3.Conv2d   512   7   7  2048   7   7              1048576  0.05MB  102660096            0.93%
    115           layer4.1.bn3.BatchNorm2d  2048   7   7  2048   7   7                 4096  0.05MB     401408            0.12%
    116                 layer4.1.relu.ReLU  2048   7   7  2048   7   7                    0  0.05MB     100352            0.09%
    117              layer4.2.conv1.Conv2d  2048   7   7   512   7   7              1048576  0.01MB  102735360            0.99%
    118           layer4.2.bn1.BatchNorm2d   512   7   7   512   7   7                 1024  0.01MB     100352            0.03%
    119              layer4.2.conv2.Conv2d   512   7   7   512   7   7              2359296  0.01MB  231185920            2.59%
    120           layer4.2.bn2.BatchNorm2d   512   7   7   512   7   7                 1024  0.01MB     100352            0.03%
    121              layer4.2.conv3.Conv2d   512   7   7  2048   7   7              1048576  0.05MB  102660096            0.99%
    122           layer4.2.bn3.BatchNorm2d  2048   7   7  2048   7   7                 4096  0.05MB     401408            0.23%
    123                 layer4.2.relu.ReLU  2048   7   7  2048   7   7                    0  0.05MB     100352            0.06%
    124                  avgpool.AvgPool2d  2048   7   7  2048   1   1                    0  0.01MB     100352            1.12%
    125                          fc.Linear          2048          1000              2049000  0.00MB    4095000            0.06%
    ===========================================================================================================================
    total parameters quantity: 25,557,032
    total memory: 4.12MB
    total MAdd: 8,219,737,624
