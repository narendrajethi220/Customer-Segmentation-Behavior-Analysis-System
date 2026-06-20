## 📌 Project Overview

Businesses collect large amounts of customer data but often do not know how different customers behave.

This project applies unsupervised learning techniques to discover hidden customer patterns and create meaningful customer segments.

The objective is to:

- Identify different customer groups
- Understand customer behaviour patterns
- Compare clustering techniques
- Visualize customer relationships using dimensionality reduction   

Pipeline:
    Raw Data

        |
    
    Drop CustomerID

        |

    Encode Gender

        |

    Scale Features

        |

      PCA

       |

     KMeans

       |

     DBSCAN

       |

   Hierarchical

       |

    Compare