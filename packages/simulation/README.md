# @repo/simulation

Simulation layer for API calls and data generation for demonstration purposes.

## Purpose

Provide realistic data and API responses without requiring actual backend services:

- Generate realistic demo data
- Simulate API latency and responses
- Create error scenarios for testing
- Mock external service integrations
- Enable offline development

## Features

- 🎲 Realistic data generation
- ⏱️ Configurable latency simulation
- 🔄 Stateful simulations (optional)
- ❌ Error scenario testing
- 📊 Time-series data generation
- 🎯 Customizable data patterns

## Usage

```typescript
import { 
  simulateRevenueData, 
  simulateApiCall,
  generateUserData 
} from '@repo/simulation';

// Generate revenue data
const revenueData = simulateRevenueData({
  days: 30,
  averageDaily: 5000,
  variance: 0.2,
});

// Simulate API call with delay
const user = await simulateApiCall(
  () => generateUserData(),
  { delay: 500 } // 500ms delay
);

// Simulate error scenario
try {
  await simulateApiCall(
    () => fetchData(),
    { errorRate: 0.3 } // 30% chance of error
  );
} catch (error) {
  // Handle simulated error
}
```

## Simulation Types

### Revenue Simulation

- Daily/monthly revenue patterns
- Seasonal variations
- Growth trends
- Anomaly injection

### Operations Simulation

- Real-time metrics
- System health status
- Performance indicators
- Incident generation

### User Behavior Simulation

- User actions and events
- Session data
- Activity patterns

## Configuration

```typescript
interface SimulationConfig {
  delay?: number;           // API latency in ms
  errorRate?: number;       // Error probability (0-1)
  cacheResults?: boolean;   // Enable result caching
  seed?: number;           // Random seed for reproducibility
}
```

## Benefits

- ✅ No backend required for demos
- ✅ Consistent demo experience
- ✅ Test error handling
- ✅ Fast development iteration
- ✅ Offline development capability

## Future Enhancements

- Record/replay actual API responses
- GraphQL simulation support
- WebSocket simulation
- Database simulation layer
