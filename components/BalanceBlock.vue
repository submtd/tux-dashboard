<template>
    <div class="card h-100">
        <div class="card-body">
            <h5 class="card-title mb-5">Balances</h5>
            <table class="table card-text">
                <tbody>
                    <tr>
                        <th scope="row">ETH</th>
                        <td>{{ useNumberFormat(ethBalance) }}</td>
                    </tr>
                    <tr>
                        <th scope="row">USDC</th>
                        <td>{{ useNumberFormat(usdcBalance) }}</td>
                    </tr>
                    <tr>
                        <th scope="row">TUX</th>
                        <td>{{ useNumberFormat(tuxBalance) }}</td>
                    </tr>
                    <tr>
                        <th scope="row">Collateral Vault</th>
                        <td>{{ useNumberFormat(collateralBalance) }}</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</template>

<script setup>
    const ethBalance = useState('ethBalance', () => 0);
    const usdcBalance = useState('usdcBalance', () => 0);
    const tuxBalance = useState('tuxBalance', () => 0);
    const collateralBalance = useState('collateralBalance', () => 0);
</script>
