# market_trader
## Summary
Market trader file takes in stock market data from alpaca api for chosen assets. In this case 'SPY','QQQ','UUP','GLD', and 'USO' though due to time constraints only SPY, UUP, and GLD were used in the decision tree and random forest machine learning models. The goal was to determine if machine learning can be used to determine the best time to use a particular algorithmic trading strategy. This program uses rolling average and RSI. 

### Data and Analysis
Rolling average was calculated as a standard indicator and RSI was chosen as a counter indicator. 
#### Decision Trees:
	GLD: Good accuracy generally between 50-60%. This model has much better accuracy predicting positive movements vs negative. The highest overall accuracy appears at a depth of 3 with 5 features at 60%. Overall accuracy generally trends down after this peak.
	UUP: Low overall accuracy under 50%. This model has higher accuracy predicting negative changes vs positive. The highest overall accuracy appears at a depth of 6 with 1 feature at 53%. Overall accuracy generally trends down after this peak.
	SPY: Good accuracy generally between 55-60%. This model has much better accuracy predicting positive movements vs negative. The highest overall accuracy appears at a depth of 5 with 3 features at 62%. Overall accuracy generally trends down after this peak.

#### Random Forest:
	GLD:  Good accuracy generally between 55-60%. This model has much better accuracy predicting positive movements vs negative. The highest overall accuracy appears at a depth of 1 with 4 features at 60%. Overall accuracy generally trends down after this peak.
	UUP:   Good accuracy generally between 55-60%. This model has much better accuracy predicting positive movements vs negative. The highest overall accuracy appears at a depth of 1 with 4 features at 60%. Overall accuracy generally trends down after this peak.
	SPY:  Good accuracy generally between 55-60%. This model has much better accuracy predicting positive movements vs negative. The highest overall accuracy appears at a depth of 1 with 4 features at 62%. Overall accuracy generally trends down after this peak.
	
### Conclusions
While this analysis is limited we can draw the conclusion that simple decision trees appear to predict positive market movements with higher accuracy for GLD and SPY assets than random forests. The random forest did show higher accuracy predicting price movements for UUP asset vs a simple decision tree the consistency of the random forest results across all assets suggests the data may be overfit. Further anaylsis of feature importance could yield different results. 
