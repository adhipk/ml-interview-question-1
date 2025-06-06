

### **Context (Anonymized Scenario)**

You are joining a team building a mobile application that recognizes physical consumer products and ensures they are scanned in the real world (not via screen images or printouts). The app runs on iOS and Android devices and integrates a visual recognition SDK that includes:

1. A product image classifier for a very large catalog.
    
2. A verification mechanism to distinguish real-world 3D objects from 2D representations.
    

We’re exploring lightweight, on-device models to ensure fast inference and offline usability.


### **Exercise 1: Image Classification Strategy Discussion (20–25 mins)**

#### Prompt:

You're tasked with designing an image classification pipeline for mobile devices that can eventually scale to 10,000+ categories. The current dataset includes images from 100 categories, captured in varied lighting and backgrounds.

#### Discussion Goals:

- Describe an architecture that would work well for mobile deployment.
    
- Suggest data augmentation strategies to improve model generalization.
    
- Talk through how you would scale this from 100 to 10,000+ classes.
    
- What are your top concerns around performance, class imbalance, and label noise?
    

---

### **Exercise 2: Real vs. Spoof Detection Design (20–25 mins)**

#### Prompt:

To prevent spoofing (e.g., using photos on a phone screen), we need a method to verify that the object being scanned is 3D and physically present. The mobile device only has a single RGB camera.

#### Design Challenge:

- Propose a strategy for real-time detection of 3D objects using monocular input (static or video).
    
- What techniques or signals could help differentiate real-world scenes from 2D fakes?
    
- How would you handle noisy input or user movement?
    

---

### **Exercise 3: On-Device Optimization & Deployment (15–20 mins)**

#### Prompt:

After model training, you need to deploy the models on iOS and Android devices with the constraint that inference should be fast and work offline.

#### Discussion Topics:

- Which formats and tools would you use for deploying on-device models?
    
- How would you optimize the model for size and latency?
    
- What trade-offs would you make during quantization or pruning?
    

---

## **Evaluation Criteria**

- System design clarity and technical depth
    
- Awareness of mobile constraints and best practices
    
- Familiarity with CV models and anti-spoofing strategies
    
- Communication, assumptions, and tradeoff analysis
    

---

Let me know if you'd like this adapted for:

- **Panel-style interviews** with role-based focuses (e.g., applied scientist vs ML infra engineer)
    
- **Pair programming variants** with partial code templates
    
- **Shorter screening rounds** with a narrowed scope
    

I can also prepare a scoring rubric or supplementary visuals if needed.