<script lang="ts">
  type ModifierProps = {
    /**
     * Numeric bonus or penalty that the situation gives to the roll
     */
    bonus?: number

    /**
     * Description of the situation that gives that bonus
     */
    situation: string
  }

  let { bonus, situation }: ModifierProps = $props()

  let displayedBonus: string = $derived.by(() => {
    if (bonus === undefined) {
      return "*"
    }

    const bonusDigits = Math.abs(bonus)
    if (bonus < 0) {
      return `–${bonusDigits}`
    }
    if (bonus === 0) {
      return "—"
    }
    if (bonus > 0) {
      return `+${bonusDigits}`
    }

    return "*"
  })
</script>

<tr><td>{displayedBonus}</td><td>{situation}</td></tr>
