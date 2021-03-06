### 3.1.12.0

- Add `MonadFail` instance for `ParsecT`
- Add `Semigroup`/`Monoid` instances for `ParsecT` (#80,#82)
- Fix space leak in Applicative/Monad interface (#37)

### 3.1.11

- Include `README.md` in package.

### 3.1.10

- Most types now have a `Typeable` instance. Some instances are dropped from
  older versions of GHC (sorry about that!).
- The token-parser now rejects Unicode numeric escape sequences for characters
  outside the Unicode range.
- The token-parser now loses less precision when parsing literal doubles.
- Documentation fixes and corrections.
- We no longer test parsec builds on GHC 7.4.

### 3.1.9

- Many and various updates to documentation and package description (inlcuding
  the homepage links).
- Add an `Eq` instance for `ParseError`
- Fixed a regression from 3.1.6: `runP` is again exported from module
  Text.Parsec.

### 3.1.8

- Fix a regression from 3.1.6 related to exports from the main module.

### 3.1.7

- Fix a regression from 3.1.6 related to the reported position of error messages.
  See bug #9 for details.
- Reset the current error position on success of `lookAhead`.

### 3.1.6

- Export `Text` instances from Text.Parsec
- Make Text.Parsec exports more visible
- Re-arrange Text.Parsec exports
- Add functions `crlf` and `endOfLine` to Text.Parsec.Char for handling
  input streams that do not have normalized line terminators.
- Fix off-by-one error in Token.charControl

### 3.1.4

- Relax dependency on `text`

### 3.1.5

- Relax dependency on `text`

### 3.1.3

- Fix a regression introduced in 3.1.2 related to positions reported by error messages.
