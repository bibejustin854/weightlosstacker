# weightlosstacker
function calculateWeightLoss(initialWeight, targetWeight) {
    /**
     * This function calculates the weight loss between an initial weight and a target weight.
     * 
     * @param {number} initialWeight - The initial weight in kilograms.
     * @param {number} targetWeight - The target weight in kilograms.
     * @returns {number} - The weight loss in kilograms.
     */
    
    try {
        // Check if both arguments are numbers
        if (typeof initialWeight !== 'number' || typeof targetWeight !== 'number') {
            throw new TypeError('Both arguments must be numbers');
        }
        
        // Calculate and return the weight loss
        return initialWeight - targetWeight;
    } catch (error) {
        // Log the error
        console.error('Error:', error.message);
        return 0;
    }
}
